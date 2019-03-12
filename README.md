# HelloWorld
实验一：Android开发基础

1.创建Hello World工程并同步GitHub

2.验证Activity的生命周期 

关键代码：

MainActivity.java

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.i("MainActivityLife","调用onCreate()");
    }
    @Override
    protected void onStart(){
        super.onStart();
        Log.i("MainActivityLife","调用onStart()");
    }
    @Override
    protected void onResume(){
        super.onResume();
        Log.i("MainActivityLife","调用onResume()");
    }
    @Override
    protected void onPause(){
        super.onPause();
        Log.i("MainActivityLife","调用onPause()");
    }
    @Override
    protected void onStop(){
        super.onStop();
        Log.i("MainActivityLife","调用OnStop()");
    }
    @Override
    protected void onDestroy(){
        super.onDestroy();
        Log.i("MainActivityLife","调用OnDestroy()");
    }
    @Override
    protected void onRestart(){
        super.onRestart();
        Log.i("MainActivityLife","调用onRestroy()");
    }
}

结果截图：


