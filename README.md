# first_app_kusminova_sidorkina
Разработчики: Кусьминова, Сидоркина
import android.widget.Button //импортируем класс кнопок чтобы потом работать с кнопками
import android.widget.TextView //импортируем класс текста
import kotlin.random.Random //импортируем фукнционал рандома

val resultTextView: TextView = findViewById(R.id.textView)  //в переменную класса TextView помещаем текст, который находим по айди.

val button: Button = findViewById(R.id.button) //в переменную класса Button помещаем нашу кнопку,которую находим по айди.

button.setOnClickListener{ //создаем "слушателя" событий нашей кнопки для реализации рандома по нажатию.
            val randomNumber = Random.nextInt(1,7) //в переменную помещается число от 1 до 7 не включительно
            resultTextView.text = "$randomNumber" //выводим в текст нашу цифру
        }

