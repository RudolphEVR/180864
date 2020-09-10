---
layout: post
section-type: post
title: Programacion - Practica 1 - Operaciones de Conjuntos
category: Programming
tags: [ 'Theory' ]
---
Python Program to Illustrate Different Set Operations

  <li>1. In this example, we have defined two set variables and we have performed different set operations: union, intersection, difference and symmetric difference.,  </li>
  <li>2. To understand this example, you should have the knowledge of the following Python programming topics:  </li>
  <li>3.Python Sets  </li>
  <li>4. Python Input, Output and Import  </li>
  <li>Python offers a datatype called set whose elements must be unique. It can be used to perform different set operations like union, intersection, difference and symmetric difference. </li>
  <li>Is the Quadratic Allocation Problem NP-complete or is it in P? Either give a reduction to show it is NP-complete or give a polytime algorithm to solve it. </li>

 
</ol>
Aside: This problem arose during some consulting I was doing, where the integers represented the sizes of different software jobs, and the quadratic term is there because the cost of implementing software goes up faster than linearly with the size of the job. 
<p></p>

<p></p>
Source Code

<pre><code data-trim class="yaml">
# - 180864-conjuntos.py *- coding: utf-8 -*-
"""
Set Section
# Program to perform different set operations like in mathematics
"""
#Find to similar command to other language
#Rust, F# and Perl
    
# define three sets
 A = set([1,2,3,4,5]) 
 B = set([3,4,5,6,7]) 
 C = {}

#%%
#pertenencia
def pertenencia():
    A = set([1,2,3,4,5]) 
    1 in A
    1 not in A 
    10 in A 
    10 not in A 
    
#%%
#Convertir a un conjunto
def transformarConj():
    A = (1,2,3)
    conjuntoA = set (A) # Set() 
    print("The set is:", conjuntoA)
    B={1,2,3,4,5}
    conjuntoB = set (B)
    print("The set B is : ", conjuntoB)
    C='Hola mundo'
    conjuntoC = set (C)
    print("The set C is :", conjuntoC)

#%%
#Quitar un elemento al conjunto
def quitar():
    A = set([0,1,2,3,4,5]) 
    A.discard(2)
    print("The set after to delete: ", A)

#%%
#Quitar todos los elementos de un conjunto
def clearSet():
    A = set([0,1,2,3,4,5]) 
    A.clear() 
    print("The set clear: ", A)

#%%
#Copiar un conjunto
def copiar():
    A = set([1,2,3,4,5]) 
    B=A.copy() 
    print("Set A = ", A, " compare set B = ", B)

#%%Agregar un elemento
def agregar():
    B.add(987) 
    print("The new set B = ", B) 
#%%%
"""
Set Operations
"""
#%%
#Unión
def union():
    A = set([1,2,3,4,5]) 
    B = set([3,4,5,6,7]) 
    print("The union = ", A|B) 
    print("The union = ", A.union(B))
#%%
#Interseccion
def intereseccion():
    A = set([1,2,3,4,5]) 
    B = set([3,4,5,6,7]) 
    print("The intersection = ", A&B)
    print(A.intersection(B))

#%%
#Diferencia
def diferencia():
    A = set([1,2,3,4,5]) 
    B = set([3,4,5,6,7]) 
    print("The diference = ", A-B)
    print("The intersection = ", A.difference(B))

#%%
#Diferencia simetrica
def simetrica():
    A = set([1,2,3,4,5]) 
    B = set([3,4,5,6,7]) 
    C = {}
    print("The symmetric_difference = ", A^B)
    
    print("The symmetric_difference = ",A.symmetric_difference(B))
    print("The symmetric_difference = ",B.symmetric_difference(A))
    print("The symmetric_difference = ",A.symmetric_difference(C))
    print("The symmetric_difference = ",B.symmetric_difference(C))

#%%
#Subconjunto
def subconjunto():
    B = set([0, 1, 2, 3, 4, 5, 6, 7, 8, 9]) 
    A = set([1,2,3,4,5]) 
    print("The subset = ",A.issubset(B) 
    print("The subset = ",B.issubset(A)

#%%
#Superconjunto
def superconjunto():
    B = set([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])
    A = set([1,2,3,4,5])
    print("The superset = ",B.issuperset(A)
    print("The supersrt = ",A.issuperset(B) 



"""
Python has lists. The empty list is []. The following is a list of one
item ["a"] and so is [3]. Here is a list with 3 items ["ball",3.14,-2]. Let's
define a list, I'll call it lis and we'll do things with it to illustrate
accessing items in a list. Execute the following cell with Ctrl-Enter.
"""

</code></pre>

<pre><code data-trim class="yaml">
email: "juancarlos.gonzalez@upslp.edu.mx"
</code></pre>

In this program, we take two different sets and perform different set operations on them. This can equivalently done by using set methods.
<small> <a href="" target="\_blank">@</a> for this feature!</small>


Visit [https://github.com/upslp-teoriacomputacional/180864/](Programming Set in Python) and you are ready to start hacking around your { Personal } website!

<small>Many thanks to <a href="https://github.com/jc-gi" target="\_blank">@jc-gi</a> for the language support! </small>
