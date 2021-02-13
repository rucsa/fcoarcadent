<template>
    <div class="footer flex flex-row blue">
        <div class="footer-menu">
            <ul class="nav w-100">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">Despre</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Preturi</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Servicii</a>
                    </li>

                </ul>
        </div>
        <div class="signature">
            <p>{{copyrights}}</p>
        </div>
        <div class="call-to-action">
            <h3 class="h3">{{actionText}}</h3>
        </div>
    </div>
</template>
<script>
export default {
    name: 'Footer',
    data () {
        return {
            copyrights: '@2020 Cabinet Stomatologic Filofteia Coarca | Created by Vulpix',
            actionText: '+4 0724 545 168',
        }
    }
}
</script>
<style scoped>
.footer {
    height: 123px;
}
</style>