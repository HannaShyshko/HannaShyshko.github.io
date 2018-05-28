TRAVEL

The idea of the cite is to provide some information about the countries and to make it real for travel lovers to realize their dreams to visit a favorite country.

The main page consists of:
- the navigation menu across the cite;
- a slide show;
- and the block of continents to observe

When the user clicks one of the blocks, he\she is redirected to the Tours page.

The Tours page consists of the blocks of countries. When the user hovers the block -> its opacity transforms from 0.6 to 1 which helps to highlight the country. The user can also learn more about the country by clicking the link in the bottom of the country block.

The Contacts page consists of two parts:

- The form (to receive the user's information)
- The contacts of the travel agency

The form consists of several inputs, some of them are necessary to fill in. The inputs also have the 'placeholder' attribute to help the user fill in the correct information. 

The cite is adaptive to the desktops and mobile phones. 



TRAVEL

Идея сайта состоит в том, чтобы помочь пользователю выбрать страну, которую он хотел бы посетить. 

На главной странице находятся заглавие, слайдшоу и блоки с конинентами (по клику на ссылку в кружке осуществляется переход на страницу со странами выбранного континента). Слайдшоу работает с помощью функции, реализованной на javascript:

<script>
var slideIndex = 0;
var carousel();

  function carousel() {
     var i;
     var x = document.getElementsByClassName("slide");
        for (i = 0; i < x.length; i++) {
          x[i].style.display = "none";
    }
       slideIndex++;
          if (slideIndex > x.length) { slideIndex = 1 }
             x[slideIndex - 1].style.display = "block";
             setTimeout(carousel, 9000);
  }
 </script>

На странице tours распологаются блоки, в которых находятся картинки и некоторая информация о стране. по умолчанию все блоки немного "в тумане" благодаря свойству opacity. при наведении на блок картинка и текст становятся ярче. внизу блока располагается ссылка. по ней можно пройти, если пользователь хочет узнать больше информации о стране. так как сайт не является реальным работающим тулом, то ссылка ведет на другую внутреннюю страницу сайта (contacts). 

На странице contacts пользователю предлагается оставить некоторую информацию о себе, заполнив форму. форма состоит из нескольких инпутов, в том числе обязательных для заполнения (для этого используем аттрибут required), также в инпутах присутствует аттрибут placeholder - подсказка для пользователя, что нужно ввести. при клике на поле, текст аттрибута placeholder исчезает. после заполнения полей пользователю предлагается отправить форму, кликнув на кнопку submit. 
Справа от формы располагается карта, по которой можно найти агентство. так как сайт не является реальным, элемент на карте был выбран рандомно. чуть выше карты располагаются номер телефона и адрес: также не реальны!
В футере страницы можно найти ссылки на соц сети в виде иконок. 

Сайт также представлен и в мобильной версии:

Главная страница состоит из блоков континентов. по клику на ссылку в блоке можно перейти на новую страницу.
на новой странице каждый блок занимает все место на экране. функционал такой: по клику на картинку свойство opacity переходит в 1. по клику на линку осуществляется переход на страницу contacts. 
на странице contacts сначала пользователь видит форму для обратной связи, после него номер телефона и адрес фирмы, ниже карта и иконки соц сетей. 
