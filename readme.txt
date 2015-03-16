1. In updatePositions(), cache ScrollTop value so we don't have to re-calculate it everytime.

2. In DOMContentLoaded listener, only add mover in visiable viewport. Since mover class has display as fixed, there is no need to paint outside the visiable area.

3. In changePizzaSizes(), cache document.querySelectorAll(".randomPizzaContainer") to avoid repetitive computation.
   Also, since the width is all the same for all pizza, we can move the new_width calculation outside the loop.