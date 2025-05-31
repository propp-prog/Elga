# Вы можете расположить сценарий своей игры в этом файле.

# Определение персонажей игры.
define e = Character('Эльга', color="#062ffa")

image forest_house="bg/forest_house.jpg"


# Вместо использования оператора image можете просто
# складывать все ваши файлы изображений в папку images.
# Например, сцену bg room можно вызвать файлом "bg room.png",
# а eileen happy — "eileen happy.webp", и тогда они появятся в игре.

#Картинки Эльги
image Elga_chil = "person/Эльга_чил.png"
image Elga_grusni = "person/Эльга_грусни.png"

# Игра начинается здесь:
label start:
    scene forest_house

    show Elga_chil

    e "Я Эльга - дочь охотника Сольди-га. Моя мама умерла и спустя время папа нашел новую жену"
    hide Elga_chil

    show Elga_grusni
    e "Папа очень любил меня и делал мне различные игрушки из дерева. Я мечтала о луке и стрелах, из-за этого мачеха невзлюбила меня "
    hide Elga_grusni


    return
