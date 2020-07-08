<template>
    <div class="profile">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-6">
                    <div class="media text-left">
                        <img src="../assets/photo.jpg" class="user-pic mr-3">
                        <div class="media-body">
                            <h5 class="mt-0">{{ firstName }} {{ lastName }}</h5>
                            {{ bio }}
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    import 'bootstrap/dist/css/bootstrap.css';

    export default {
        name: 'Profile',
        data: function () {
            return {
                firstName: 'Lyodra',
                lastName: 'Margaretha Ginting',
                bio: 'Lahir di Medan, 21 Juni 2003. adalah seorang penyanyi asal Medan, Sumatra Utara, Indonesia.'
            }
        },
        components: {}
    }
</script>

<style scoped>
    .user-pic {
        border-radius: 200px;
        height: 80px;
        width: 80px;
    }
</style>