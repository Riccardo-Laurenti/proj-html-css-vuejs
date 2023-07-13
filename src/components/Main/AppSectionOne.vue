<script>
import ServiceCard from './SectionOne/ServiceCard.vue';


export default{
    data() {
        return {
            ArrServices:[
                {
                    id:1,
                    //image:'src/assets/quickwind/i.png',
                    text: 'Our History',
                    title: 'Founded by a worldwide-famous yacht racer Alfred Tannenstrick,since its inception back in 1977, this company has been a welcoming harbor for all yachting and sailing enthusiasts,from all across the US!',
                    description: 'We offer a real variety of professional services, from the simple yachts chartering and corporate events, all the way to yacht repairs, upgrades and modifications and maintenance checkups.',
                    seconddescription: 'With decades of professional experience in renting, repairing and transporting just all kinds of yachts and boats under our belt – we can assure you that we are your best choice! ',
                },
            ]
        }
    },
    components:{
        ServiceCard,
    }
};
</script>

<template>
    <section class="first_section">
        <div class="">
            <div class=" ">
                <div class="d-flex justify-content-end">
                    <div class="col-6 " style="width: 31%; margin-right: 430px">
                        <div class="index">
                            <ServiceCard 
                            v-for="service in ArrServices"
                            :key="service.id"
                            :image="service.image"
                            :text="service.text"
                            :title="service.title"
                            :description="service.description"
                            :seconddescription="service.seconddescription"
                            />
                        </div>
                        <button class=" button_nav py-2 rounded-1 me-3 border-0" style="color:white; font-weight: 600; background-color: #16a9bd;">
                            Read More
                        </button>
                    </div>
                </div>
            </div>
        </div>  
    </section>

    
</template>

<style lang="scss" scoped>
    .first_section {
        height: 1100px;
        background-image: url(./../../assets/quickwind/images/bg4.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }

    .container{

    }

    .button_nav{
        padding-inline: 2rem;
    }

    .first_title_main{
        padding-top: 6rem;
    }

    .container_col{

        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }


    .index{

    }


    .sub_col3{

    }

    
    
</style>