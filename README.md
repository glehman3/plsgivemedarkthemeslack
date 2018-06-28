WE ALL WANT DARK THEME
PLEASE
SLACK


//

Add snippet to bottom of ssb-interop.js for full dark theme goodness.


`document.addEventListener('DOMContentLoaded', function() {
 $.ajax({
   url: 'https://cdn.rawgit.com/glehman3/plsgivemedarkthemeslack/f20ad19c/cssthatslackcantdo',
   success: function(css) {
      css += `
     
           div.c-virtual_list__scroll_container {
           background-color: #222 !important;
       }
       .p-message_pane .c-message_list:not(.c-virtual_list--scrollbar), .p-message_pane .c-message_list.c-virtual_list--scrollbar > .c-scrollbar__hider {
            z-index: 0;
       }
       div.c-message__content:hover {
           background-color: #2F2C2F !important;
       }

       div.c-message:hover {
           background-color: #2F2C2F !important;
       }
     `;
     $("<style></style>").appendTo('head').html(css);
   }
 });
});

//

Side bar color code for manual slack preferences: #222222,#252525,#A36B31,#D2D6D6,#5C6380,#DEDEDE,#ADBA4E,#DB6668

