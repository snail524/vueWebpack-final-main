<template>
    <div>
        <header class="navbar navbar-dark sticky-top bg-dark flex-md-nowrap p-0 shadow">
        <a class="navbar-brand col-md-3 col-lg-2 me-0 px-3" href="#">Borrow Mountain</a>
        <button class="navbar-toggler position-absolute d-md-none collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#sidebarMenu" aria-controls="sidebarMenu" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
        </button>
        <input class="form-control form-control-dark w-100" type="text" placeholder="Search" aria-label="Search">
        <div class="navbar-nav">
            <div class="nav-item text-nowrap">
            <a class="nav-link px-3" href="#" @click.prevent="signout">Sign out</a>
            </div>
        </div>
        </header>
    </div>
</template>

<script>
export default {
    name: 'Navnar',
    methods:{
        signout(){
            const vm = this;
            const api = `${process.env.APIPATH}/logout`;
            this.$http.post(api).then((response) => {
            console.log(response.data);
            // 回到login頁面
            if(response.data.success){
                vm.$router.push('/signin');  // 頁面轉回
            }
            });
    }
    }
}
</script>

