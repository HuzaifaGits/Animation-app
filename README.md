# Animation-app
java code

package com.example.aniamtionapp;

import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.view.animation.Animation;
import android.view.animation.AnimationUtils;
import android.widget.Button;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {
   TextView anim;
    Button btn1;
    Button btn2;
    Button btn3;
    Button btn4;
    Button btn5;
    Button btn6;
    Button btn7;
    Button btn8;
    Button btn9;
    Button btn10;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        anim=findViewById(R.id.textView3);
        btn1=findViewById(R.id.button);
        btn2=findViewById(R.id.button2);
        btn3=findViewById(R.id.button3);
        btn4=findViewById(R.id.button4);
        btn5=findViewById(R.id.button5);
        btn6=findViewById(R.id.button6);
        btn7=findViewById(R.id.button7);
        btn8=findViewById(R.id.button8);
        btn9=findViewById(R.id.button9);
        btn10=findViewById(R.id.button12);






        btn1.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation rotate =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.rotate);
                anim.startAnimation(rotate);
            }
        });
        btn2.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation slidedown =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.slidedown);
                anim.startAnimation(slidedown);
            }
        });
        btn3.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation fade =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.fade);
                anim.startAnimation(fade);
            }
        });
        btn4.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation blink =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.blink);
                anim.startAnimation(blink);
            }
        });
        btn5.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation move =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.move);
                anim.startAnimation(move);
            }
        });
        btn6.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation slide =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.slide);
                anim.startAnimation(slide);
            }
        });
        btn7.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation zoomin =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.zoomin);
                anim.startAnimation(zoomin);

            }});
        btn8.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation bounce =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.bounce);
                anim.startAnimation(bounce);
            }
        });
        btn9.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation clockwise =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.clockwise);
                anim.startAnimation(clockwise);
            }
        });


        btn10.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Animation close =
                        AnimationUtils.loadAnimation(getApplicationContext(), R.anim.close);
                anim.startAnimation(close);
            }
        });
}}
