<template>
    <a href="#" v-on:click="topFunction" id="myBtn" class="fixed-bottom text-decoration-none go-to">
        <span class="justify-content-center align-items-center p-2">
            Scroll to top
            <img src="@/assets/icons/Vector 9.png" alt="No Image">
        </span>
    </a>
</template>

<script>
export default {
    name:'GoTo',
    methods:{
        topFunction()
        {
            document.body.scrollTop = 0;
            document.documentElement.scrollTop = 0;
        }
    },
    mounted()
    {
        // Get the button
        let mybutton = document.getElementById("myBtn");
        mybutton.style.display = "none";
        
        // When the user scrolls down 20px from the top of the document, show the button
        window.onscroll = function() {scrollFunction()};
        
        function scrollFunction() {
          if (document.body.scrollTop > 1 || document.documentElement.scrollTop > 1) {
            mybutton.style.display = "block";
          } else {
            mybutton.style.display = "none";
          }
        }
    }
}
</script>