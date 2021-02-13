<template>
    <div class="button-custom">
        <a
           :href="to" 
           >{{buttonTitle}}</a>
    </div>
</template>
<script>
export default {
    name: 'Button',
    props: {
        anchor: false,
        buttonTitle: null,
        to: null,
        textColor: 'red',
        fontSize: 30,
        buttonClass: 'button-custom',
        fontWeigth: 800
    }
}
</script>
<style scoped>
a {
    font-family: 'Montserrat';
    padding: .5em 2.5em;
    font-size: .8em;
    font-weight: 800;
    background: #F2B705 0% 0% no-repeat padding-box;
    border-radius: 15px;
    opacity: 1;

}
</style>