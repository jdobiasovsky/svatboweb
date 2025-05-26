---
layout: page
title: Kdy to bude?
permalink: /when/
---

## Svoje ano si řekneme 30.srpna

Více informací najdeš v programu.

<p class="timer"> Do svatby zbývá:</p>
<p id="timer-clock" class="timer"></p>

<!-- Display the countdown timer in an element -->
<script>
// Set the date we're counting down to
var countDownDate = new Date("Aug 30, 2025 12:30:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

    // Get today's date and time
    var now = new Date().getTime();

    // Find the distance between now and the count down date
    var distance = countDownDate - now;

    // Time calculations for days, hours, minutes and seconds
    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);

    // Display the result in the element with id="timer-clock"
    document.getElementById("timer-clock").innerHTML = days + "d " + hours + "h " +
        minutes + "m " + seconds + "s ";

    // If the count down is finished, write some text
    if (distance < 0) {
        clearInterval(x);
        document.getElementById("timer-clock").innerHTML = "Nic. Konečně svoji!";
    }
}, 1000);
</script>
