---
layout: default
---


## Stenokeyboard
Sep 2025 - Nov 2025


<div style="display: grid; grid-template-columns: repeat(6, 1fr); gap: 10px; max-width: 240px; margin-bottom: 24px;">
    <img src="assets/img/stm32cubeide-logo.png" alt="STM32CubeIDE" style="width: 28px;">

    <img src="assets/img/altium-logo.png" alt="Altium Designer" style="width: 120px;">
    <img src="assets/img/usb2.png" alt="UBC Rocket" style="width: 50px;">
</div>


<script>
    function toggleContent(buttonElement) {
        // 1. Get the ID of the content block to target from the button's data attribute
        const targetId = buttonElement.getAttribute('data-target');
        const contentBlock = document.getElementById(targetId);

        // 2. Get the text container within the button (where the text is located)
        const textContainer = buttonElement.querySelector('.button-text');
        
        // 3. Toggle the display property
        if (contentBlock.style.display === 'none' || contentBlock.style.display === '') {
            // SHOW
            // The image container uses 'display: flex' internally for the carousel layout, 
            // but the outer container should use 'block' to appear on a new line.
            contentBlock.style.display = 'block'; 
            
            // Check if the content inside the contentBlock should be flex
            contentBlock.querySelector('div').style.display = 'flex'; 
        } else {
            // HIDE
            contentBlock.style.display = 'none';
        }
    }
</script>

<div style="display: flex; gap: 20px; margin-bottom: 20px;"> 
    <div 
        class="toggle-button"
        onclick="toggleContent(this)" 
        data-target="image-testing"
        style="
            display: flex;
            padding: 0;
            background-color: #f0f0f0;
            border-radius: 8px; 
            color: inherit;  
            width: 150px; 
            cursor: pointer; 
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); 
        ">
        <div class="button-text" style="
          padding: 10px; 
          flex-grow: 1;
          text-align: center; 
          font-weight: bold;
        ">
          Development
        </div>
    </div>

    <div 
        class="toggle-button"
        onclick="toggleContent(this)" 
        data-target="image-soldering"
        style="
            display: flex;
            padding: 0;
            background-color: #f0f0f0;
            border-radius: 8px; 
            color: inherit; 
            width: 150px; 
            cursor: pointer; 
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); 
        ">
        <div class="button-text" style="
          padding: 10px; 
          flex-grow: 1;
          text-align: center; 
          font-weight: bold;
        ">
          Soldering
        </div>
    </div>

</div> 
<div id="image-testing" style="display: none; margin-top: 10px;">
    <img src="/assets/img/Steno/Testing.png" alt="Testing the keyboard module" style="border-radius: 10px; height: 400px;">
</div>

<div id="image-soldering" style="display: none; margin-top: 10px;">
    <img src="/assets/img/Steno/soldering.png" alt="Steno PCB" style="height: 400px; border-radius: 10px;">
</div>

Working on it!

[Back](./AESN.html)
