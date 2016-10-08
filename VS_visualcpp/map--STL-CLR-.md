---
title: "map (STL-CLR)"
ms.custom: na
ms.date: 10/03/2016
ms.devlang: 
  - C++
ms.prod: visual-studio-dev14
ms.reviewer: na
ms.suite: na
ms.technology: 
  - devlang-cpp
ms.tgt_pltfrm: na
ms.topic: reference
H1: map (STL/CLR)
ms.assetid: 8b0a7764-b5e4-4175-a802-82b72eb8662a
caps.latest.revision: 18
manager: ghogen
translation.priority.ht: 
  - cs-cz
  - de-de
  - es-es
  - fr-fr
  - it-it
  - ja-jp
  - ko-kr
  - pl-pl
  - pt-br
  - ru-ru
  - tr-tr
  - zh-cn
  - zh-tw
---
# map (STL-CLR)
The template class describes an object that controls a varying-length sequence of elements that has bidirectional access. You use the container `map` to manage a sequence of elements as a (nearly) balanced ordered tree of nodes, each storing one element. An element consists of a key, for ordering the sequence, and a mapped value, which goes along for the ride.  
  
 In the description below, `GValue` is the same as:  
  
 `Microsoft::VisualC::StlClr::GenericPair<GKey, GMapped>`  
  
 where:  
  
 `GKey` is the same as `Key` unless the latter is a ref type, in which case it is `Key^`  
  
 `GMapped` is the same as `Mapped` unless the latter is a ref type, in which case it is `Mapped^`  
  
## Syntax  
  
```  
template<typename Key,  
    typename Mapped>  
    ref class map  
        :   public  
        System::ICloneable,  
        System::Collections::IEnumerable,  
        System::Collections::ICollection,  
        System::Collections::Generic::IEnumerable<GValue>,  
        System::Collections::Generic::ICollection<GValue>,  
        System::Collections::Generic::IList<GValue>,  
        System::Collections::Generic::IDictionary<Gkey, GMapped>,  
        Microsoft::VisualC::StlClr::ITree<Gkey, GValue>  
    { ..... };  
```  
  
#### Parameters  
 Key  
 The type of the key component of an element in the controlled sequence.  
  
 Mapped  
 The type of the additional component of an element in the controlled sequence.  
  
## Members  
  
|Type Definition|Description|  
|---------------------|-----------------|  
|[map::const_iterator (STL/CLR)](../VS_visualcpp/map--const_iterator--STL-CLR-.md)|The type of a constant iterator for the controlled sequence.|  
|[map::const_reference (STL/CLR)](../VS_visualcpp/map--const_reference--STL-CLR-.md)|The type of a constant reference to an element.|  
|[map::const_reverse_iterator (STL/CLR)](../VS_visualcpp/map--const_reverse_iterator--STL-CLR-.md)|The type of a constant reverse iterator for the controlled sequence.|  
|[map::difference_type (STL/CLR)](../VS_visualcpp/map--difference_type--STL-CLR-.md)|The type of a (possibly signed) distance between two elements.|  
|[map::generic_container (STL/CLR)](../VS_visualcpp/map--generic_container--STL-CLR-.md)|The type of the generic interface for the container.|  
|[map::generic_iterator (STL/CLR)](../VS_visualcpp/map--generic_iterator--STL-CLR-.md)|The type of an iterator for the generic interface for the container.|  
|[map::generic_reverse_iterator (STL/CLR)](../VS_visualcpp/map--generic_reverse_iterator--STL-CLR-.md)|The type of a reverse iterator for the generic interface for the container.|  
|[map::generic_value (STL/CLR)](../VS_visualcpp/map--generic_value--STL-CLR-.md)|The type of an element for the generic interface for the container.|  
|[map::iterator (STL/CLR)](../VS_visualcpp/map--iterator--STL-CLR-.md)|The type of an iterator for the controlled sequence.|  
|[map::key_compare (STL/CLR)](../VS_visualcpp/map--key_compare--STL-CLR-.md)|The ordering delegate for two keys.|  
|[map::key_type (STL/CLR)](../VS_visualcpp/map--key_type--STL-CLR-.md)|The type of an ordering key.|  
|[map::mapped_type (STL/CLR)](../VS_visualcpp/map--mapped_type--STL-CLR-.md)|The type of the mapped value associated with each key.|  
|[map::reference (STL/CLR)](../VS_visualcpp/map--reference--STL-CLR-.md)|The type of a reference to an element.|  
|[map::reverse_iterator (STL/CLR)](../VS_visualcpp/map--reverse_iterator--STL-CLR-.md)|The type of a reverse iterator for the controlled sequence.|  
|[map::size_type (STL/CLR)](../VS_visualcpp/map--size_type--STL-CLR-.md)|The type of a (non-negative) distance between two elements.|  
|[map::value_compare (STL/CLR)](../VS_visualcpp/map--value_compare--STL-CLR-.md)|The ordering delegate for two element values.|  
|[map::value_type (STL/CLR)](../VS_visualcpp/map--value_type--STL-CLR-.md)|The type of an element.|  
  
|Member Function|Description|  
|---------------------|-----------------|  
|[map::begin (STL/CLR)](../VS_visualcpp/map--begin--STL-CLR-.md)|Designates the beginning of the controlled sequence.|  
|[map::clear (STL/CLR)](../VS_visualcpp/map--clear--STL-CLR-.md)|Removes all elements.|  
|[map::count (STL/CLR)](../VS_visualcpp/map--count--STL-CLR-.md)|Counts elements matching a specified key.|  
|[map::empty (STL/CLR)](../VS_visualcpp/map--empty--STL-CLR-.md)|Tests whether no elements are present.|  
|[map::end (STL/CLR)](../VS_visualcpp/map--end--STL-CLR-.md)|Designates the end of the controlled sequence.|  
|[map::equal_range (STL/CLR)](../VS_visualcpp/map--equal_range--STL-CLR-.md)|Finds range that matches a specified key.|  
|[map::erase (STL/CLR)](../VS_visualcpp/map--erase--STL-CLR-.md)|Removes elements at specified positions.|  
|[map::find (STL/CLR)](../VS_visualcpp/map--find--STL-CLR-.md)|Finds an element that matches a specified key.|  
|[map::insert (STL/CLR)](../VS_visualcpp/map--insert--STL-CLR-.md)|Adds elements.|  
|[map::key_comp (STL/CLR)](../VS_visualcpp/map--key_comp--STL-CLR-.md)|Copies the ordering delegate for two keys.|  
|[map::lower_bound (STL/CLR)](../VS_visualcpp/map--lower_bound--STL-CLR-.md)|Finds beginning of range that matches a specified key.|  
|[map::make_value (STL/CLR)](../VS_visualcpp/map--make_value--STL-CLR-.md)|Constructs a value object.|  
|[map::map (STL/CLR)](../VS_visualcpp/map--map--STL-CLR-.md)|Constructs a container object.|  
|[map::rbegin (STL/CLR)](../VS_visualcpp/map--rbegin--STL-CLR-.md)|Designates the beginning of the reversed controlled sequence.|  
|[map::rend (STL/CLR)](../VS_visualcpp/map--rend--STL-CLR-.md)|Designates the end of the reversed controlled sequence.|  
|[map::size (STL/CLR)](../VS_visualcpp/map--size--STL-CLR-.md)|Counts the number of elements.|  
|[map::swap (STL/CLR)](../VS_visualcpp/map--swap--STL-CLR-.md)|Swaps the contents of two containers.|  
|[map::to_array (STL/CLR)](../VS_visualcpp/map--to_array--STL-CLR-.md)|Copies the controlled sequence to a new array.|  
|[map::upper_bound (STL/CLR)](../VS_visualcpp/map--upper_bound--STL-CLR-.md)|Finds end of range that matches a specified key.|  
|[map::value_comp (STL/CLR)](../VS_visualcpp/map--value_comp--STL-CLR-.md)|Copies the ordering delegate for two element values.|  
  
|Operator|Description|  
|--------------|-----------------|  
|[map::operator= (STL/CLR)](../VS_visualcpp/map--operator=--STL-CLR-.md)|Replaces the controlled sequence.|  
|[map::operator(STL/CLR)](../VS_visualcpp/map--operator-STL-CLR-.md)|Maps a key to its associated mapped value.|  
|[operator!= (map) (STL/CLR)](../VS_visualcpp/operator!=--map---STL-CLR-.md)|Determines if a `map` object is not equal to another `map` object.|  
|[operator< (map) (STL/CLR)](../VS_visualcpp/operator---map---STL-CLR-.md)|Determines if a `map` object is less than another `map` object.|  
|[operator<= (map) (STL/CLR)](../VS_visualcpp/operator-=--map---STL-CLR-.md)|Determines if a `map` object is less than or equal to another `map` object.|  
|[operator== (map) (STL/CLR)](../VS_visualcpp/operator==--map---STL-CLR-.md)|Determines if a `map` object is equal to another `map` object.|  
|[operator> (map) (STL/CLR)](../VS_visualcpp/operator---map---STL-CLR-.md)|Determines if a `map` object is greater than another `map` object.|  
|[operator>= (map) (STL/CLR)](../VS_visualcpp/operator-=--map---STL-CLR-.md)|Determines if a `map` object is greater than or equal to another `map` object.|  
  
## Interfaces  
  
|Interface|Description|  
|---------------|-----------------|  
|<xref:System.ICloneable?qualifyHint=False>|Duplicate an object.|  
|<xref:System.Collections.IEnumerable?qualifyHint=False>|Sequence through elements.|  
|<xref:System.Collections.ICollection?qualifyHint=False>|Maintain group of elements.|  
|<xref:System.Collections.Generic.IEnumerable`1?qualifyHint=False>|Sequence through typed elements.|  
|<xref:System.Collections.Generic.ICollection`1?qualifyHint=False>|Maintain group of typed elements.|  
|<xref:System.Collections.Generic.IDictionary`2?qualifyHint=False>|Maintain group of {key, value} pairs.|  
|ITree<Key, Value>|Maintain generic container.|  
  
## Remarks  
 The object allocates and frees storage for the sequence it controls as individual nodes. It inserts elements into a (nearly) balanced tree that it keeps ordered by altering the links between nodes, never by copying the contents of one node to another. That means you can insert and remove elements freely without disturbing remaining elements.  
  
 The object orders the sequence it controls by calling a stored delegate object of type [map::key_compare (STL/CLR)](../VS_visualcpp/map--key_compare--STL-CLR-.md). You can specify the stored delegate object when you construct the map; if you specify no delegate object, the default is the comparison `operator<(key_type, key_type)`. You access this stored object by calling the member function [map::key_comp (STL/CLR)](../VS_visualcpp/map--key_comp--STL-CLR-.md)`()`.  
  
 Such a delegate object must impose a strict weak ordering on keys of type [map::key_type (STL/CLR)](../VS_visualcpp/map--key_type--STL-CLR-.md). That means, for any two keys `X` and `Y`:  
  
 `key_comp()(X, Y)` returns the same Boolean result on every call.  
  
 If `key_comp()(X, Y)` is true, then `key_comp()(Y, X)` must be false.  
  
 If `key_comp()(X, Y)` is true, then `X` is said to be ordered before `Y`.  
  
 If `!key_comp()(X, Y) && !key_comp()(Y, X)` is true, then `X` and `Y` are said to have equivalent ordering.  
  
 For any element `X` that precedes `Y` in the controlled sequence, `key_comp()(Y, X)` is false. (For the default delegate object, keys never decrease in value.) Unlike template class [map](../VS_visualcpp/map--STL-CLR-.md), an object of template class `map` does not require that keys for all elements are unique. (Two or more keys can have equivalent ordering.)  
  
 Each element contains a separate key and a mapped value. The sequence is represented in a way that permits lookup, insertion, and removal of an arbitrary element with a number of operations proportional to the logarithm of the number of elements in the sequence (logarithmic time). Moreover, inserting an element invalidates no iterators, and removing an element invalidates only those iterators which point at the removed element.  
  
 A map supports bidirectional iterators, which means you can step to adjacent elements given an iterator that designates an element in the controlled sequence. A special head node corresponds to the iterator returned by [map::end (STL/CLR)](../VS_visualcpp/map--end--STL-CLR-.md)`()`. You can decrement this iterator to reach the last element in the controlled sequence, if present. You can increment a map iterator to reach the head node, and it will then compare equal to `end()`. But you cannot dereference the iterator returned by `end()`.  
  
 Note that you cannot refer to a map element directly given its numerical position -- that requires a random-access iterator.  
  
 A map iterator stores a handle to its associated map node, which in turn stores a handle to its associated container. You can use iterators only with their associated container objects. A map iterator remains valid so long as its associated map node is associated with some map. Moreover, a valid iterator is dereferencable -- you can use it to access or alter the element value it designates -- so long as it is not equal to `end()`.  
  
 Erasing or removing an element calls the destructor for its stored value. Destroying the container erases all elements. Thus, a container whose element type is a ref class ensures that no elements outlive the container. Note, however, that a container of handles does `not` destroy its elements.  
  
## Requirements  
 **Header:** <cliext/map>  
  
 **Namespace:** cliext  
  
## See Also  
 [hash_map (STL/CLR)](../VS_visualcpp/hash_map--STL-CLR-.md)   
 [hash_map (STL/CLR)](../VS_visualcpp/hash_map--STL-CLR-.md)   
 [hash_multiset (STL/CLR)](../VS_visualcpp/hash_multiset--STL-CLR-.md)   
 [hash_set (STL/CLR)](../VS_visualcpp/hash_set--STL-CLR-.md)   
 [map](../VS_visualcpp/map--STL-CLR-.md)   
 [multiset (STL/CLR)](../VS_visualcpp/multiset--STL-CLR-.md)   
 [set (STL/CLR)](../VS_visualcpp/set--STL-CLR-.md)   
 [STL/CLR Library Reference](../VS_visualcpp/STL-CLR-Library-Reference.md)