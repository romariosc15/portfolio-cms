<template>
    <div class="h-screen p-6 space-y-4 shadow-md bg-white">
        <div class="">
            <h4 class="text-2xl font-extrabold">CMS</h4>
        </div>
        <div class="space-y-2">
            <h6 class="text-sm font-light text-gray-400">SECCIONES</h6>
            <div class="flex flex-col space-y-1">
                <NuxtLink to="/experience">
                    <div class="px-4 py-2 rounded-md hover:bg-blue-400 hover:text-white text-gray-600 space-x-2 flex">
                        <svg-icon type="mdi" :path="experienceIcon"></svg-icon> 
                        <span>Experiencia</span>
                    </div>
                </NuxtLink>
                <NuxtLink to="/portfolio">
                    <div class="px-4 py-2 rounded-md hover:bg-blue-400 hover:text-white text-gray-600 space-x-2 flex">
                        <svg-icon type="mdi" :path="portfolioIcon"></svg-icon> 
                        <span>Portafolio</span>
                    </div>
                </NuxtLink>
                <NuxtLink to="/contact">
                    <div class="px-4 py-2 rounded-md hover:bg-blue-400 hover:text-white text-gray-600 space-x-2 flex">
                        <svg-icon type="mdi" :path="contactIcon"></svg-icon> 
                        <span>Contacto</span>
                    </div>
                </NuxtLink>
            </div>
        </div>
    </div>
</template>

<script>
    import SvgIcon from '@jamescoyle/vue-icon';
    import { mdiAccountTie, mdiFileDocumentOutline, mdiPhone } from '@mdi/js';
    
    export default {
        components: {
            SvgIcon
        },
        data() {
        return {
            experienceIcon: mdiAccountTie,
            portfolioIcon: mdiFileDocumentOutline,
            contactIcon: mdiPhone
        }
    }
    }
</script>