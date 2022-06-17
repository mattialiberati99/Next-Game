<template>
    <div class="SectionLogo">
        <div :class="active?'active hamburger-menu':'hamburger-menu'" @click="active=!active">
            <div class="bar top"></div>
            <div class="bar middle"></div>
            <div class="bar bottom"></div>
        </div>
        <svg width="98" height="53" viewBox="0 0 98 53" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path
                d="M84.5801 14.0144H90.4988V31.9448C90.4988 33.5792 89.1739 34.9041 87.5395 34.9041C85.905 34.9041 84.5801 33.5792 84.5801 31.9448V14.0144Z"
                fill="#333333" />
            <rect x="77.0947" y="14.0144" width="5.91876" height="20.8897" rx="2.95938"
                transform="rotate(-90 77.0947 14.0144)" fill="#333333" />
            <path
                d="M61.8628 11.0551C61.8628 9.42067 63.1878 8.0957 64.8222 8.0957C66.4566 8.0957 67.7816 9.42066 67.7816 11.0551V28.9854H61.8628V11.0551Z"
                fill="#333333" />
            <path
                d="M67.7816 34.9042C64.5127 34.9042 61.8628 32.2543 61.8628 28.9854H79.7931C81.4276 28.9854 82.7525 30.3104 82.7525 31.9448C82.7525 33.5792 81.4276 34.9042 79.7931 34.9042H67.7816Z"
                fill="#333333" />
            <path
                d="M54.1162 11.0551C54.1162 9.42067 55.4412 8.0957 57.0756 8.0957C58.71 8.0957 60.035 9.42066 60.035 11.0551V28.9854H54.1162V11.0551Z"
                fill="#333333" />
            <path
                d="M54.1159 34.9042C57.3847 34.9042 60.0347 32.2543 60.0347 28.9854L39.1449 28.9854C39.1449 32.2543 41.7949 34.9042 45.0637 34.9042H54.1159Z"
                fill="#333333" />
            <path
                d="M39.145 11.0551C39.145 9.42067 40.47 8.0957 42.1044 8.0957C43.7388 8.0957 45.0638 9.42066 45.0638 11.0551V28.9854H39.145V11.0551Z"
                fill="#333333" />
            <path d="M26.3983 4L32.243 18.3617H20.5536L26.3983 4Z" fill="#F46119" />
            <path
                d="M19.2402 14.2031L29.0186 16.8232C34.419 18.2703 37.6239 23.8212 36.1768 29.2217C34.7298 34.6221 29.1788 37.827 23.7784 36.3799C18.3779 34.9329 15.1731 29.3819 16.6201 23.9815L19.2402 14.2031Z"
                fill="#F46119" />
            <path
                d="M33.5566 14.2031L36.1767 23.9815C37.6238 29.3819 34.4189 34.9329 29.0185 36.3799C23.6181 37.827 18.0671 34.6221 16.6201 29.2217C15.173 23.8212 18.3779 18.2703 23.7783 16.8232L33.5566 14.2031Z"
                fill="#F46119" />
            <g filter="url(#filter0_d_1_3834)">
                <circle cx="26.3985" cy="26.6015" r="6.09284" fill="white" />
            </g>
            <circle cx="25.3179" cy="26.8159" r="1.09669" fill="#F46119" fill-opacity="0.25" />
            <circle cx="28.0273" cy="26.8159" r="0.548345" fill="#F46119" fill-opacity="0.25" />
            <defs>
                <filter id="filter0_d_1_3834" x="0.305664" y="0.508667" width="52.1855" height="52.1857"
                    filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
                    <feFlood flood-opacity="0" result="BackgroundImageFix" />
                    <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
                        result="hardAlpha" />
                    <feMorphology radius="5" operator="dilate" in="SourceAlpha" result="effect1_dropShadow_1_3834" />
                    <feOffset />
                    <feGaussianBlur stdDeviation="7.5" />
                    <feComposite in2="hardAlpha" operator="out" />
                    <feColorMatrix type="matrix" values="0 0 0 0 1 0 0 0 0 1 0 0 0 0 1 0 0 0 0.15 0" />
                    <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_1_3834" />
                    <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_1_3834" result="shape" />
                </filter>
            </defs>
        </svg>

    </div>
</template>
<script>
    export default {
    data (){
        return {
            active:true
        }
    }
}
</script>
<style>
.SectionLogo {
    margin-top: 20px;
    margin-bottom: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.SectionLogo .icon {
    width: 24px;
    height: 24px;
    border-radius: 100%;
    background-color: var(--light6);
    margin-right: 10px;
}

.SectionLogo svg {
    margin-right: 30px;
}
.hamburger-menu {
  display: flex;
  flex-flow: column wrap;
  justify-content: space-between;
  height: 24px;
  width: 24px;
  margin-left: -6px;
  cursor: pointer;
}

.hamburger-menu .bar {
  height: 2px;
  background: var(--light6);
  border-radius: 2px;
  margin: 3px 0px;
  transform-origin: left;
  transition: all 0.5s;
}

.hamburger-menu.active .top {
  transform: rotate(45deg);
}

.hamburger-menu.active .middle {
  opacity: 0;
}

.hamburger-menu.active .bottom {
  transform: rotate(-45deg);
}
</style>