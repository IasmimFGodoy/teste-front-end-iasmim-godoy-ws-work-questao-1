<template>
    <div class="carousel-container">
        <button id="arrow-left" class="control">◀</button>
        <div class="gallery-wrapper">
            <figure>
                <img id="Carousel-img1" src="Carousel-img1.jpg" alt="First food of Carousel">
                <figcaption><h3>$ 8.77</h3></figcaption>
            </figure>
            <figure>
                <img id="Carousel-img2" src="Carousel-img2.jpg" alt="First food of Carousel">
                <figcaption><h3>$ 8.77</h3></figcaption>
            </figure>
            <figure>
                <img id="Carousel-img3" src="Carousel-img3.jpg" alt="First food of Carousel">
                <figcaption><h3>$ 8.77</h3></figcaption>
            </figure>
            <figure>
                <img id="Carousel-img4" src="Carousel-img4.jpg" alt="First food of Carousel">
                <figcaption><h3>$ 8.77</h3></figcaption>
            </figure>
            
        </div>
        <button id="arrow-right" class="control">▶</button>
    </div>
</template>
<script>
import { onMounted } from 'vue';
export default {
    setup() {
    
        onMounted(() => {
            const images = document.querySelectorAll(".gallery-wrapper img");
            let currentImageIndex = 0;

            document.querySelector("#arrow-left").addEventListener("click", () => {
                images[currentImageIndex].style.border = "none";
                currentImageIndex--;
                if (currentImageIndex < 0) {
                    currentImageIndex = images.length - 1;
                }
                images[currentImageIndex].style.border = "3px solid #285943";
            });

            document.querySelector("#arrow-right").addEventListener("click", () => {
                images[currentImageIndex].style.border = "none";
                currentImageIndex++;
                if (currentImageIndex >= images.length) {
                    currentImageIndex = 0;
                }
                images[currentImageIndex].style.border = "3px solid #285943";
            });
        });
  },
};
</script>
<style>
.carousel-container {
    background-color: #D7FFF1;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 600px;
    height: 110px;
    border: 1px solid black;
    margin-left: 1rem;
    margin-top: 1rem;
}
.gallery-wrapper {
    display: flex;
}
#arrow-left {
    margin-left: 0.5rem;
}
#arrow-right {
    margin-right: 0.5rem;
}
#arrow-left, #arrow-right {
    background-color: transparent;
    border: none;
    font-size: 24px;
}
#arrow-left:hover, #arrow-right:hover {
    cursor: pointer;
}
.gallery-wrapper {
    margin-top: 1rem;
}
.gallery-wrapper h3{
    margin-left: 1.5rem;
}
#Carousel-img1, #Carousel-img2, #Carousel-img3, #Carousel-img4{
    margin-right: 1rem;
}
#Carousel-img1 {
    width: 125px;
    border: 3px solid #285943;
}
#Carousel-img2 {
    width: 100px;
    height: 60px;
}
#Carousel-img3{
    width: 100px;
    height: 60px;
}
#Carousel-img4 {
    margin-left: 1rem;
    height: 60px;
}

</style>