<template>
    <div>
        <section class="hero">
            <b-container>
                <b-row class="text-center">
                    <b-col>
                        <div class="hero__heading">
                            <h1>Private Cloud</h1>
                        </div>
                    </b-col>
                </b-row>
            </b-container>
        </section>
        <section class="about">
            <b-container>
                <b-row class="justify-content-center text-center">
                    <b-col sm="12" md="8">
                        <h1 class="heading">How Private Cloud Helps Your Business</h1>
                    </b-col>
                </b-row>
                <b-row class="justify-content-md-center">
                    <b-col sm="12" md="10">
                        <p>Get the agility, scalability and efficiency of the public cloud, with the greater levels of control and security of a single-tenant, dedicated environment. It can be hosted on-site at your own data center or at a service provider’s data center.</p>
                    </b-col>
                </b-row>
                <b-row class="justify-content-center">
                    <b-col csm="12" md="10">
                        <h5 class="page__title">Use Cases</h5>
                        <p>Choose a private cloud when security, control and performance are your top priority.</p>
                    </b-col>
                </b-row>
                <b-row class="justify-content-center">
                    <b-col sm="12" md="10">
                        <ul class="page__text">
                            <li>Workloads and data with demanding security requirements </li>
                            <li>Mission-critical business applications</li>
                            <li>Addressing compliance regulations </li>
                            <li>Data sovereignty</li>
                            <li>Applications that require high performance</li>
                            <li>Data center consolidation and extension</li>
                            <li>IT-as-a-service</li>
                            <li>Test/dev environments and application development</li>
                            <li>Disaster recovery</li>
                        </ul>
                    </b-col>
                </b-row>
                <b-row class="justify-content-md-center text-center custom">
                    <b-col>
                        <b-btn @click="show=true" class="btn btn-bg-dark">Request FREE Quote</b-btn>
                        <b-modal v-model="show" hide-footer="true">
                            <div class="require-form">
                                <contact-form></contact-form>
                            </div>
                        </b-modal>
                    </b-col>
                </b-row>
            </b-container>
        </section>
        <section class="page">
            <b-container>
                <b-row>
                    <b-col sm="12" md class="page__card">
                        <img class="page__img" src="../assets/images/agility.svg" />
                        <h5 class="page__title">Agility</h5>
                        <p class="page__text">Deliver features faster by providing your users with on-demand, self-service access to infrastructure.</p>
                    </b-col>
                    <b-col sm="12" md class="page__card">
                        <img class="page__img" src="../assets/images/icon-cloud.svg" />
                        <h5 class="page__title">Security</h5>
                        <p class="page__text">Get the enhanced security of dedicated, physically isolated network, compute and storage layers.</p>
                    </b-col>
                    <b-col sm="12" md class="page__card">
                        <img class="page__img" src="../assets/images/customization.svg" />
                        <h5 class="page__title">Customization</h5>
                        <p class="page__text">Customize the dedicated compute, storage and networking components to best suit your needs.</p>
                    </b-col>
                    <b-col sm="12" md class="page__card">
                        <img class="page__img" src="../assets/images/performance.svg" />
                        <h5 class="page__title">Performance</h5>
                        <p class="page__text">Gain performance advantages over public cloud, with dedicated resources for your business.</p>
                    </b-col>
                </b-row>
            </b-container>
        </section>
    </div>
</template>

<script>
import ContactForm from '@/components/contact-form'

export default {
    name: 'PrivateCloud',
    metaInfo: {
		meta: [
		  { name: 'description', content: 'Get the agility, scalability and efficiency of the public cloud, with the greater levels of control and security of a single-tenant, dedicated environment.' },
		  { name: 'keywords', content: 'private cloud, private cloud for business, platops private cloud' }
		]
	},
    components: {
        ContactForm
    },
    data () {
        return {
            show: false
        }
    }
}
</script>

<style lang="scss" scoped>

.page__list {
    li {
        padding: 10px 0;
    }
}

.custom {
    margin: 15px 0;
}

@media screen and (max-width: 767px) {
    .custom {
        margin-bottom: -40px;
    }

    .page__card {
        padding: 20px 25px;
    }
}
</style>
