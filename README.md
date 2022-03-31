# Report

I have replaced the previous text for today's date, which is then displayed onto the screen.

Note that the XML-file, _content_main_, now refers to another resource, namely _strings.xml_. From there, the text 'Today is' can be obtained. Today's date is then appended to this string, as can be seen from the code snippet below:

```java
TextView textView = findViewById(R.id.currentDate);
String date = new SimpleDateFormat("EEEE, dd/MM/yyyy", Locale.getDefault()).format(new Date());
textView.setText(textView.getText() + ": " + date);
```

<p align="center">
  <img src="screenshot.png" alt="screenshot" width="400px"/>
</p>
