# Accordion
Accordion

$(document).on('click', '.accordion-toggle', function() {
    var parent = $(this).closest('.accordion');
    
    // Remove active class from all elements
    parent.find('.accordion-toggle').removeClass('in');
    parent.find('.accordion-body').removeClass('in');
    
    // Add class to specific elements
    $(this).addClass('in');
    $(this).next('.accordion-body').addClass('in');
});
