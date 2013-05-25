TrainYourBrain
==============

Наша верзија на српскиот квиз Слагалица, со ново руво и нов шмек. Одлична игра доколку сакате да ја подобрите кондицијата на вашиот мозок :D

Изработена од:

Даринка Буровска 113005

Марија Граматикова 113008

Даница Николоска 113045

**Train Your Brain** е логичка игра, со која може да ги испробате вашите интелектуални вештини и способности.  Можете да го тестирате вашиот речник, вашата способност за брзо сметање, логичко размислување и вашите општи познавања од повеќе сфери. Играта се состои од повеќе делови и секој дел има одредена тежина каде можете да тестирате различни способности. 

![poceten ekran](http://i.imgur.com/NVgIcPK.png)

Почетниот екран е организиран со 5 копчиња за секоја од игрите и до секое од нив лабела за освоениот резултат. Играчот може да си избира по кој редослед ги игра игрите, меѓутоа крајниот резултат ќе му се впише дури откако ке ги одгира сите 5 игри. Во секој момент може да побара нова игра од грното мени, со тоа што повторно ќе му се активираат сите 5 копчиња за избор на игра. Исто така од горното мени може да одбере да ја види листата со најдобри резултати, да ги прочита правилата за секоја игра, и доколку не е задоволен од моменталниот изглед на играта, да си одбере соодветен излгед од неколкуте понудени.


## Мој Збор
Целта на играчот е да состави колку што е можно подолг збор. Со креирање на формата се одбираат 10 букви. Секоја буква има толку веројатност да се појави, колку што е нејзината фреквенцијата во македонската азбука. Со самото прикажување на формата се стартува тајмер, кој е прикажан како пита. Питата е имплементирана со функциите за графика. Зборот се составува со кликање на копчињата или пак со куцање од тастатурата, со тоа што може да се внесат букви кои биле генерирани. Со кликање на крај се проверува текстуалната датотека дали го содржи зборот кој е внесен, и во одност на најден најдолг збор кој може да се состави со тие букви,се доделуваат поени.  Доколку нема подолг збор од понудениот, ги добива сите поени, доколку има пократок збор му се  одземаат поени во зависност од големината на зборот. 

![moj zbor](http://i.imgur.com/0Am6Ddp.png)

## Мој број
Со самото стартување на играта се генерира рандом троцифрен број (бројот кој треба да се добие) и уште 6 други броеви (4 едноцифрени, 1 двоцифрен и 1 троцифрен). Со нивна комбинација и користење на дадените оператори потребно е да се формира математички израз чиј резултат ќе биде еднаков на дадениот троцифрен број погоре. Ако е исполнет тој услов играчот освојува 100 поени. Во спротивно не се признава резултатот и играчот добива 0 поени. Времето е ограничено. 

![moj broj](http://i.imgur.com/otXjBm8.png)


## Погоди ме


Со помош на 6те симболи дадени во долниот дел од погледот, треба да се погоди комбинацијата од 4 рандом генерирани симболи. Доколку симболот го има во комбинацијата, меѓутоа не е на правилно место тоа се означува со бело кругче. А доколку симболот е на точната позиција тогаш се исцртува црно кругче. Во случај на грешка играчот има право да го промени избраниот симбол, со еден клик над него. Корекции на потегот се можни само пред да се кликне на копчето “Потврди”. Играчот има право на 6 обиди, и дополнително временско ограничување. 
Копчето потврди се активира само кога ќе се внесе комбинација од 4 симболи. По клик на копчето се проверува комбинациајта во функцијата Check(), а потоа со функцијата PaintBall() се исцртуваат црните и белите кругчиња.
Кратко објаснување на функцијата Check():
при секој повик на функцијата "замислената" комбинација се сместува во помошна низа која служи за проверка. Со првиот for циклус се изминува цела низа е се споредува со помошната низа(низа од тековно испратените симболи). Доколу точно погоден симбол, се бори, и се продолжува понатаму. Со вториот for циклус идентично на првиот се проверува цела низа, меѓутоа овој пат се бараат симболите што ги има во комбинацијата меѓутоа не се на правилно место. 

![pogodi me](http://i.imgur.com/jCCIlIt.png)

## Слагалица

Играта претставува копија на детските игри, каде една слика е поделена на NxN полиња и едно од полето е извадено и овозможува останатите да се разместат. Целта на играта е да ги да ги подреди броевите од 1 до 9 кои се генерирани рандом и се  разместени. На случаен начин се одбира едно кое ќе биде извадено. Полињата претставуваат копчиња чиј текст е бројката што го претставува кое поле е. Поместувањето се врши на клик на копче. Доколку еден од соседите негови (горе долу лево или десно) е невидлив кликнатото копче со невидливото си ги променуваат броевите, и кликнатото станува невидливо, а невидливото се појавува. За секое од копчињата кое содржи бројка неговите соседи се чуваат во Мапа (Dictionary) со клуч Button,  а вредност листа од Button, за да можеме брзо и лесно да ги најдеме кои копчиња да ги проверувамеТајмерот кој мери е имплементиран исто како во другите делови при секое разместување на бројки се проверува дали играта е завршена успешно. 

![slagalica](http://i.imgur.com/DoG7c3L.png)

## Квиз
Потребно е играчот да одговара на поставените прашања со ДА или НЕ. Вкупно има 10 прашања на кои треба да се одговори и истите се од различна област. Колку повеќе точни одговори, толку повеќе поени. Времето е ограничено.
За квизот имаме помошна класа Prasanje која чува податоци за прашањето и неговиот одговор. Прашањата се генерираат по случаен редослед со повикување на функцијата Novo(). При секој клик на некое од копчињата ДА или НЕ се проверува точноста на одговорот, со тоа се ажурира и резултатот од точно одговорените прашања и повторно се повикува функцијата за генерирање на ново прашање. 

![kviz](http://i.imgur.com/k6Stc3b.png)


