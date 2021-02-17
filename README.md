# 3D-Carousel-ReactJs

A resposive and customizable carousel for reactJs

## Get Started

### npm
    npm i t-a-e-3d-carousel-reactjs

## information

| Parameter        | Type     | Default | Description                                                                      |
|------------------|----------|---------|----------------------------------------------------------------------------------|
| imageList        | List     | null    | List of images url/path and title (optional)                                     |
| autoplay         | Boolean  | false   | Automatically change image slides                                                |
| showArrows       | Boolean  | true    | Side arrows display status                                                       |
| interval         | Integer  | 2000    | If autoplay is enabled, the time period in milliseconds of image slides changing |
| className        | String   | null    | carousel class name                                                              |
| imageClassName   | String   | null    | carousel images class name                                                       |
| onClick          | function | null    | on click function                                                                |
| overlayClassName | String   | null    | carousel image overlay class name                                                |
| id               | String   | null    | carousel id                                                                      |

#### parameter usage
    <Carousel 
        imageList={List}
        autoplay={Boolean}
        showArrows={Boolean}
        interval={Integer}
        className={String}
        imageClassName={String}
        onClick={function}
        overlayClassName={String}
        id={String}
        >


### usage
    import { Carousel } from 't-a-e-3d-carousel-reactjs'

    function App () {

        const Images = {
            {
                title: 'title 1',
                url: 'https://images.unsplash.com/photo-1492144534655-ae79c964c9d7?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxzZWFyY2h8MXx8Y2Fyc3xlbnwwfHwwfA%3D%3D&auto=format&fit=crop&w=500&q=60'
            },
            {
                title: 'title 2',
                url: 'https://images.unsplash.com/photo-1583121274602-3e2820c69888?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1050&q=80'
            },
            {
                title: '',
                url: 'https://images.unsplash.com/photo-1517672651691-24622a91b550?ixlib=rb-1.2.1&ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&auto=format&fit=crop&w=1189&q=80'
            },
        }

     return (
         <Carousel imageList={Images} />
     )   
    }

    export default App