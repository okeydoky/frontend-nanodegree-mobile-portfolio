1. In updatePositions(), cache ScrollTop value so we don't have to re-calculate it everytime.

2. In changePizzaSizes(), cache document.querySelectorAll(".randomPizzaContainer") to avoid repetitive computation.

3. In DOMContentLoaded listener, only add mover in visiable viewport. Since mover class has display as fixed, there is no need to paint outside the visiable area.