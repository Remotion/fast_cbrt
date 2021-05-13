# Fast cbrt(x).

One way to compute cube root is this:

    float cbrt(float x) { return x < 0.0f ? -pow(-x, 1.0f/3.0f) : pow(x, 1.0f/3.0f); };

But this is probably the worst way to do it, because pow() is usually pretty slow. Precision is not that great either.
Fortunately, there are faster ways to compute cube root. Precision can also be higher as naive pow() implementation.  

In this repository I am trying to show some of them.
