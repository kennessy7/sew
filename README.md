# 19273007 고다현

## 1주차 과제
 리눅스
 
## 2주차 과제
<img width="200" height="" src="./png/캡스톱디자인 과제(2주차)_19273007고다현.png"></img>

## 3주차 과제
<img width="200" height="" src="./png/캡스톤 과제(3주차_1)_19273007 고다현.png"></img>
<img width="200" height="" src="./png/캡스톤 과제(3주차_2)_19273007 고다현.png"></img>
<img width="200" height="" src="./png/캡스톤 과제(3주차_3)_19273007 고다현.png"></img>

## 4주차 과제

 - 아이디어 정리
  : 일과 등록/달성 관리 앱
    1) 매일 지정한 시간에 하루 일과를 입력하는 알람이 뜬다.
    2) 일과 지정 시 시작 / 종료 시간을 입력해 놓으면 해당 시간에 알람이 뜬다.
    3) 일과 완료시 완료 체크가 가능하다.
    4) 매일 지정한 시간에 하루 일과 달성 여부를 체크하라는 알람이 뜬다.
    5) 일별, 주별, 월별 달성률 리포트를 볼 수 있다.

## 7 주차과제
 - 좌측 상단에 학번 및 이름 기입 완료.
 
<img width="200" height="" src="./png/캡스톤 과제(7주차_1)_19273007 고다현.png"></img>
<img width="200" height="" src="./png/캡스톤 과제(7주차_2)_19273007 고다현.png"></img>

## 9주차과제
  - 실행 되지 않아 재 업로드 예정. 
package com.example.test_scroll2;

import androidx.appcompat.app.AppCompatActivity;

import android.content.res.Resources;
import android.graphics.drawable.BitmapDrawable;
import android.os.Bundle;
import android.view.View;
import android.widget.ImageView;
import android.widget.ScrollView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    ScrollView scrollView;
    ImageView imageView;
    BitmapDrawable bitmap;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        scrollView = findViewById(R.id.verScrollView);
        imageView = findViewById(R.id.imageView);
        scrollView.setHorizontalScrollBarEnabled(true);

        Resources res = getResources();
        bitmap = (BitmapDrawable) res.getDrawable(R.drawable.image01);
        int bitmapWidth = bitmap.getIntrinsicWidth();
        int bitmapHeight = bitmap.getIntrinsicHeight();

        imageView.setImageDrawable(bitmap);
        imageView.getLayoutParams().width = bitmapWidth;
        imageView.getLayoutParams().height = bitmapHeight;

    }
        public void btnClicked(View v)
        {
            Resources res = getResources();
            bitmap = (BitmapDrawable) res.getDrawable(R.drawable.image02);
            int bitmapWidth = bitmap.getIntrinsicWidth();
            int bitmapHeight = bitmap.getIntrinsicHeight();

            imageView.setImageDrawable(bitmap);
            imageView.getLayoutParams().width = bitmapWidth;
            imageView.getLayoutParams().height = bitmapHeight;

    }
}
