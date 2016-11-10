---
title: "How to: Write a parallel_for_each Loop"
ms.custom: na
ms.date: "10/14/2016"
ms.prod: "visual-studio-dev14"
ms.reviewer: na
ms.suite: na
ms.technology: 
  - "devlang-cpp"
ms.tgt_pltfrm: na
ms.topic: "article"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "writing a parallel_for_each loop [Concurrency Runtime]"
  - "parallel_for_each function, example"
ms.assetid: fa9c0ba6-ace0-4f88-8681-c7c1f52aff20
caps.latest.revision: 12
ms.author: "mithom"
manager: "ghogen"
translation.priority.ht: 
  - "de-de"
  - "es-es"
  - "fr-fr"
  - "it-it"
  - "ja-jp"
  - "ko-kr"
  - "ru-ru"
  - "zh-cn"
  - "zh-tw"
translation.priority.mt: 
  - "cs-cz"
  - "pl-pl"
  - "pt-br"
  - "tr-tr"
---
# How to: Write a parallel_for_each Loop
This example shows how to use the [concurrency::parallel_for_each](../Topic/parallel_for_each%20Function.md) algorithm to compute the count of prime numbers in a [std::array](../stdcpplib/array-class--stl-.md) object in parallel.  
  
## Example  
 The following example computes the count of prime numbers in an array two times. The example first uses the [std::for_each](../Topic/for_each.md) algorithm to compute the count serially. The example then uses the `parallel_for_each` algorithm to perform the same task in parallel. The example also prints to the console the time that is required to perform both computations.  
  
 [!code[concrt-parallel-count-primes#1](../parallel/codesnippet/CPP/how-to--write-a-parallel_for_each-loop_1.cpp)]  
  
 The following sample output is for a computer that has four processors.  
  
 **serial version:**  
**found 17984 prime numbers**  
**took 6115 ms**  
**parallel version:**  
**found 17984 prime numbers**  
**took 1653 ms**   
## Compiling the Code  
 To compile the code, copy it and then paste it in a Visual Studio project, or paste it in a file that is named `parallel-count-primes.cpp` and then run the following command in a Visual Studio Command Prompt window.  
  
 **cl.exe /EHsc parallel-count-primes.cpp**  
  
## Robust Programming  
 The lambda expression that the example passes to the `parallel_for_each` algorithm uses the `InterlockedIncrement` function to enable parallel iterations of the loop to increment the counter simultaneously. If you use functions such as `InterlockedIncrement` to synchronize access to shared resources, you can present performance bottlenecks in your code. You can use a lock-free synchronization mechanism, for example, the [concurrency::combinable](../parallel/combinable-class.md) class, to eliminate simultaneous access to shared resources. For an example that uses the `combinable` class in this manner, see [How to: Use combinable to Improve Performance](../parallel/how-to--use-combinable-to-improve-performance.md).  
  
## See Also  
 [Parallel Algorithms](../parallel/parallel-algorithms.md)   
 [parallel_for_each Function](../Topic/parallel_for_each%20Function.md)