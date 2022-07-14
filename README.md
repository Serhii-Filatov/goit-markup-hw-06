# goit-markup-hw-06








Форма у футері. Зверніть увагу на те, як вона там позиціонована - вона притиснута до правого краю контейнера.

Позиціонування іконок у input. В основному це така конструкція: загальний div, в якому лежить label, input та svg-іконка. Іконка позиціонується абсолютом, але щодо свого батька -- div. Input -- це сусідній елемент для іконки. Не вірно (непотрібно) буде також прописати для інпуту position: relative. Можна вгадувати позиціонування до подібної візуальної відповідності, але це теж не буде технічно правильно.

Щоб правильно спозиціонувати іконку, є кілька варіантів, але найпростіший і зрозуміліший для вас - input і svg-іконку покласти в div. Цьому контейнеру дати position:relative. svg-position:absolute. І тепер буде зрозуміле і грамотне позиціонування іконки - вона через absolute дісталася з потоку документа, а div прийняв розміри input

Коли абсолютно позиціонуєте, не забувайте, що, як правило, треба дві точки. Наприклад top та left. Навіть якщо візуально нічого не зміниться.

Не забувайте, коли ставите, наприклад top:50% - це не зовсім центр, який хочеться. Щоб він був дійсним, додавайте transform: translateY(-50%);

Не забуваймо робити фокус на кастомному чекбоксі.


