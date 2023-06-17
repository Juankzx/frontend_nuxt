<template>
<div>
    <baseAside/>
    <main class="main-content position-relative max-height-vh-100 h-100 border-radius-lg">
    
        <baseNav :page="page" :modulo="modulo"/>
    
        <div class="container-fluid py-4">
        <slot name="body" />
        <baseFooter/>
      
    </div>
    </main>
  </div>
</template>
<script>
export default{
    name: 'AdminTemplate',
    props: {
    page: {
      type: String,
      default: ''
    },
    modulo: {
      type: String,
      default: ''
    },
  }
}
</script>