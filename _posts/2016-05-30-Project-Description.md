---
layout: post
title: Project Description
comments: true
category: portfolio
tags:
    - web-development
    - jekyll
    - theme
---

## Idea ##


Nowadays, people’s lifestyles are influenced by globalization. People not only concern themselves with local news, but also focus on the international news. And specially, in some modules like politics and sports, it’s interesting to know the opinions from different countries. However, there may be a language problem for readers to get information from other opinions written in different languages. Our app will focus on this problem and provides multiple views for users.


## Use Cases ##

layout: post title: Project description comments: true category: portfolio tags: - web-development - jekyll - theme — * When a controversial call happened during a football match between two clubs from England and Spain, what are the opinions on it of the fans of the two clubs?


<p class="highlighter-header">JAVA</p>
{% highlight java linenos %}
/*
  Get Tail Map from Java TreeMap example
  This Java Example shows how to get the portion of TreeMap whose keys
  are grater than or equal to the specified key using tailMap method
  of Java TreeMap class.
*/

import java.util.SortedMap;
import java.util.TreeMap;

public class GetTailMapFromTreeMapExample {

  public static void main(String[] args) {

    //create TreeMap object
    TreeMap treeMap = new TreeMap();

    //add key value pairs to TreeMap
    treeMap.put("1","One");
    treeMap.put("3","Three");

    /*
      To get a Tail Map from Java TreeMap use,
      SortedMap tailMap(Object fromKey) method of Java TreeMap class.

      Please note that, the SortedMap returned by this method is backed by
      the original TreeMap. So any changes made to SortedMap will be
      reflected back to original TreeMap.
    */

    SortedMap sortedMap = treeMap.tailMap("2");

    System.out.println("Tail Map Contains : " + sortedMap);
  }
}
{% endhighlight %}
Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim.
Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium. Integer tincidunt. Cras dapibus. Vivamus elementum semper nisi. Aenean vulputate eleifend tellus.

