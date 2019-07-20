# ToastLib
I am learning to create android dependencies. This may be the simplest one ever. It just shows a toast message. I am getting familiarized with the procedure that's all.

### Add this to your project

Inside the root level gradle script:

```
allprojects {
	repositories {
		...
		maven { url 'https://jitpack.io' }
	}
}
```


Inside app level gradle script:

```
dependencies {
    implementation 'com.github.AshHasib:ToastLib:Tag'
}

```


### Uses

```
class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)


        MyToaster.showLongToast(this,"Hello from Nowhere!!!")

    }
}
```
  
