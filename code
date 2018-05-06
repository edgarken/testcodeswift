//Swift 
// Типы переменных
let Integer123 = 1
let String123 = "String"
let Float123: Float = 7.01
let Double123: Double = 7.01
let welcomeMessage: String
welcomeMessage = "Welcome!"
let minValue = UInt8.min // minValue равен 0, а его тип UInt8
let maxValue = UInt8.max // maxValue равен 255, а его тип UInt8
let maxValueInt = Int8.max
let minValueInt = Int8.min
let maxValueInt32 = Int32.max
let maxValueInt64 = Int64.max

/* Swift всегда будет выбирать тип Double, если он увидит число
плавающей точкой */
let pi = 3.14159
let three = 3
// Int сам превратится в Double и anotherPi будет Double
let anotherPi = 3 + 3.14159
let anotherPi2 = Double(three) + 3.14159
let anotherPi3 = three + Int(pi)

let twoThousand: UInt16 = 2_000
let one: UInt8 = 1
let twoThousandAndOne = twoThousand + UInt16(one)

// Конвертация Int в String(строку)
let label = "The width is "
let width = 94
let widthLabel = label + String(width)

// Конвертация Int в String(строку) в String'e
let apples = 5
let oranges = 2
let text1 = "My friend has \(apples) apples."
let text2 = "My friend has \(oranges) oranges."
let text3 = "My friend has \(apples + oranges) apples and oranges."

// Массивы
var shoppinglist = ["catfish", "water", "tulips", "blue paint"]
shoppinglist[0]
/* Обрати внимание, что начинается отсчет с 0, а не с 1! */
shoppinglist[1]
/* Это словарь! При вызове Malcolm нам покажут Captain */
var occupations = [
    "Malcolm": "Captain",
    "Kaylee": "Mechanic",
]
occupations["Malcolm"]
/* К словарю добавляется еще одно значение и к нему же пояснение */
occupations["Jayne"] = "Public Relations"
occupations["Jayne"]

/* Создание пустого массива */
let emptyArray = [String]()
/* Создание пустого словаря */
let emptyDictionary = [String: Float]()

/* Так же создание пустового массива и словаря */
shoppinglist = []
occupations = [:]

// Интересная штука typealias, она переименовывает что-то

typealias AudioSample = UInt16
var maxAmplitudeFound = AudioSample.min
// maxAmplitudeFound теперь 0

// Логические типы
let orangesAreOrange = true
let turnipsAreDelicious = false

if turnipsAreDelicious {
    print("Ох, репа такая вкусная!")
} else {
    print("Фу, репа ужасна на вкус!")
}

let i = 1
if i == 1 {
    // этот пример выполнится успешно
}

// Кортежи
let http404Error = (404, "Not Found")
var (statusCode, statusMessage) = http404Error
print("The status code is \(statusCode)")
print("The status message is \(statusMessage)")
print("The status code is \(http404Error.0)")
/* Если вам нужны только некоторые из значений кортежа, вы можете игнорировать части кортежа во время разложения с помощью символа подчеркивания (_) */
let (justTheStatusCode, _) = http404Error
print(justTheStatusCode)
let http200Status = (statusCode2: 200, description: "OK")
print("The status code is \(http200Status.statusCode2)")
// Выведет "The status code is 200"
print("The status message is \(http200Status.description)")
// Выведет "The status message is OK"

// Опциональный типы
let possibleNumber = "123"
let convertedNumber = Int(possibleNumber)
/* 
Int?: (Он не может содержать ничего другого, например Bool
значение или значение String. Он либо Int, либо вообще ничто)
*/

var serverResponseCode: Int? = 404
// serverResponseCode содержит реальное Int значение 404
serverResponseCode = nil
// serverResponseCode теперь не содержит значения
// Это сравнимо с var serverResponseCode: (без типа)

var surveyAnswer: String
var surveyAnswer2: String?
// surveyAnswer автоматически установится в nil
if convertedNumber != nil {
    print("convertedNumber contains some integer value.")
}

/*
 Короче, вот этот ? ставишь тогда, когда думаешь или хотя бы
предполагаешь, что у этого Типа будет nil
*/
// ВАЖНО!
/* nil != 0, nil это nil. 0 - это значение, которые было получено впоследствии присваивания или, например, 5 - 5. А nil - это вообще такого значения нет, его не существует. Как я понял, ячейка памяти вообще пуста. Типо, var lolka: string. Но почему тогда я не могу использовать var lolka: string. Все просто, друг. nil'у не может быть присвоено что-нибудь. Если присвоить, то ERROR.
*/
var numberTest1:Int? = 2
var numberTest2:Int = 2
var summanumberTest = numberTest1! + numberTest2
var lolka: String
numberTest1 = nil
//Это ошибка вызывана СПЕЦИАЛЬНО! Это чтобы ты отличал Int? и Int
numberTest2 = nil
//Это ошибка вызывана СПЕЦИАЛЬНО! Это чтобы ты отличал Int? и Int
