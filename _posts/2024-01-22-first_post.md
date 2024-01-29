---
layout: post
title:  분수꼴의 미분 - 증명 
categories: ml dl

---


{% raw %}

$1. \quad \text{Let } h(x) = \frac{1}{g(x)} \text{. We want to find } h'(x).$  

$2. \quad h'(x) = \lim_{{\Delta x \to 0}} \frac{h(x + \Delta x) - h(x)}{\Delta x}$  

$3. \quad = \lim_{{\Delta x \to 0}} \frac{\frac{1}{g(x + \Delta x)} - \frac{1}{g(x)}}{\Delta x}$  

$4. \quad = \lim_{{\Delta x \to 0}} \frac{g(x) - g(x + \Delta x)}{g(x)g(x + \Delta x)\Delta x}$  

$5. \quad = -\lim_{{\Delta x \to 0}} \frac{g(x + \Delta x) - g(x)}{g(x)g(x + \Delta x)\Delta x}$  

$6. \quad = -\frac{\lim_{{\Delta x \to 0}} \frac{g(x + \Delta x) - g(x)}{\Delta x}}{g(x)\lim_{{\Delta x \to 0}}g(x + \Delta x)}$

$7. \quad = -\frac{g'(x)}{g(x)g(x)}$  

$8. \quad = -\frac{g'(x)}{[g(x)]^2}$  

{% endraw %}
