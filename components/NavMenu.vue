<template>
    <div class="container-fluid blue flex flex-row nav-container">
        <div class="logo">
            <h1 class="h1">FCoarcaDent</h1>
        </div>
        <div class="menu">
            <ul class="nav w-100 justify-content-end">
                <li class="nav-item">
                    <a class="nav-link active" href="#">Despre</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Servicii Stomatologice</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="/preturi">Preturi</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">Contact</a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name: 'NavMenu'
    
}
</script>
<style scoped>
.nav {
    height: 50px;
}

.logo h1 {
    color: white;
}
</style>