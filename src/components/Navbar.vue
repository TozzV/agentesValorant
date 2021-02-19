<template>
    <div >
        <nav id="navbar">
      <ul class="navbar-list">
        <li class="navbar-itens">Populares</li>
        <li class="navbar-itens">Lançamentos</li>
        <li class="navbar-itens">Demais agentes</li>
      </ul>
      
    </nav>
    </div>
</template>

<script>
export default {
    props: ['navbar'],

    
}
</script>

<style scoped>

.navbar-list {
    text-align: center;
    list-style: none;
}

.navbar-itens {
    color: white;
    
    display: inline;
    padding: 5%;
}

.navbar-itens:hover {
    color: #BB3537;
}

</style>