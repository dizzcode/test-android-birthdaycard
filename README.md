# Build a simple app with text composables : Birthday Card

### Note 1
### Annotations
Annotations are means of attaching extra information to code. This information helps tools like the Jetpack Compose compiler, and other developers understand the app's code.

An annotation is applied by prefixing its name (the annotation) with the `@` character at the beginning of the declaration you are annotating. Different code elements, including properties, functions, and classes, can be annotated. Later on in the course, you'll learn about classes.

The following diagram is an example of annotated function:
> @Preview(
showBackground = true,
showSystemUi = true,
name = "App Preview"
)
@Composable
fun GreetingPreview() {
    HappyBirthdayTheme {
        Greeting("Android")
    }
}


### Composable function names
The compose function that returns nothing and bears the `@Composable` annotation MUST be named using `Pascal case`. Pascal case refers to a naming convention in which the first letter of each word in a compound word is capitalized.

https://github.com/androidx/androidx/blob/androidx-main/compose/docs/compose-api-guidelines.md#naming-unit-composable-functions-as-entities

The Compose function:  
>MUST be a noun: DoneButton()
NOT a verb or verb phrase: DrawTextField()
NOT a nouned preposition: TextFieldWithLink()
NOT an adjective: Bright()
NOT an adverb: Outside()
Nouns MAY be prefixed by descriptive adjectives: RoundIcon()  


// Do: This function is a descriptive PascalCased noun as a non-visual element
// with presence in the composition  
@Composable  
fun BackButtonHandler() {}  

// Don't: This function is neither PascalCased nor a noun!  
@Composable  
fun drawProfileImage(image: ImageAsset) {}  



