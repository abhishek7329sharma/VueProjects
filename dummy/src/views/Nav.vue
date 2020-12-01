<template>

<div class="container p-2  navabar" align="right">
<b-nav type="dark" align="right"  >
        <b-nav-item class="" ><a href="" class="nav-bar ">
            <i class="fa fa-times" aria-hidden="true"></i>
            Close</a></b-nav-item>
    </b-nav>
</div>
    
</template>
<script>
export default {
    name: 'Nav'
                }
</script>

<style >
/* navbar styling */
.navabar{
    
}
    a.nav-bar{
      color: #686b69;
      font-weight: bold;
      text-decoration: none;

      }
      a.nav-bar:hover{
      color: #505250;
      
      text-decoration: none;

      }

</style>