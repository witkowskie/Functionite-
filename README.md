# Functionite-
zadanie rekrutacyjne dla Functionite - modal box 


     ----------------------     KOMENTARZ     ---------------------- 
   
   
          1) strona posiada button do otwarcia modal-boxa, 
          bez możliwości otwarcia, modal-box nie byłby
          modal-boxem. 

          2) całe zadanie można wykonać 'łatwiej' pry użyciu 
          preprocesora CSS - np. Sass, ułatwiłoby to zapisywanie 
          powtarzających się zmiennych, jak font, kolor etc.

          3) elementy accessability są widoczne, jednak nieliczne.
          Głównie ze względu na małą złożoność strony. 
          Starałam się jednak ich użyć, zarówno w <head>,
          jak i przypisując język strony jako angielski. 
          W przykładowym tekście zaznaczyłam cytaty i ich źródło. 


          4)  vertical align - inne metody
              
              jest wiele metod centrowania w pionie, 
              zależy to głównie od tego, jakie elementy
              chcemy wycentrować. w tym przypadku jest to
              div w div'ie. możemy rozwiązać to tak:

              .parent-div {
                position: relative;
              }
              .child-div {
                position: absolute;
                top: 50%;
                height: 100px;
                margin-top: -50px; 
              }
              
              albo:
              
              .parent-div {
                position: relative;
              }
              .child-div {
                position: absolute;
                top: 50%;
                transform: translateY(-50%);
              }


              można też osiągnąć ten efekt przy użyciu flexboxa:

              .parent {
                display: flex;
                flex-direction: column;
                justify-content: center;
              }

            można też eksperymentować w zależności od tego,
            ile divów mamy w danym divie i jak względem 
            siebie i całej strony są ułożone. Co też uczyniłam. 

    ----------------------    / KOMENTARZ     ---------------------- 
   
