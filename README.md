# Прогнозирование заказов такси на следующий час
<h1>Содержание<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Прогнозирование-заказов-такси-на-следующий-час" data-toc-modified-id="Прогнозирование-заказов-такси-на-следующий-час-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Прогнозирование заказов такси на следующий час</a></span><ul class="toc-item"><li><span><a href="#Описание-проекта" data-toc-modified-id="Описание-проекта-1.1"><span class="toc-item-num">1.1&nbsp;&nbsp;</span>Описание проекта</a></span></li><li><span><a href="#Описание-данных" data-toc-modified-id="Описание-данных-1.2"><span class="toc-item-num">1.2&nbsp;&nbsp;</span>Описание данных</a></span></li><li><span><a href="#Вывод" data-toc-modified-id="Вывод-1.3"><span class="toc-item-num">1.3&nbsp;&nbsp;</span>Вывод</a></span></li></ul></li></ul></div>



## Описание проекта
Компания «Чётенькое такси» собрала исторические данные о заказах такси в аэропортах. Чтобы привлекать больше водителей в период пиковой нагрузки, нужно спрогнозировать количество заказов такси на следующий час. Постройте модель для такого предсказания.

## Описание данных
- num_orders - количество заказов

## Вывод
<table>
         <thead>
           <tr>
             <th></th>
             <th>RandomForest</th>
             <th>CatBoost</th>
             <th>LightGBM</th>
           </tr>
         </thead>
         <tbody>
           <tr>
             <th>RMSE(train)</th>
             <td>14.7502</td>
             <td>2.74705</td>
             <td>0.609076</td>
           </tr>
           <tr>
             <th>RMSE(valid)</th>
             <td>39.1047</td>
             <td>37.0475</td>
             <td>37.9111</td>
           </tr>
           <tr>
             <th>RMSE(test)</th>
             <td>47.9249</td>
             <td>46.4442</td>
             <td>45.0187</td>
           </tr>
           <tr>
             <th>Время обучения (секунды)</th>
             <td>5.2</td>
             <td>1.62</td>
             <td>1.44</td>
           </tr>
           <tr>
             <th>Время предсказания (секунды)</th>
             <td>0.0139878</td>
             <td>0.00259209</td>
             <td>0.00408912</td>
           </tr>
         </tbody>
       </table>

