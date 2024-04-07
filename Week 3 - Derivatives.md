# Week 3 - Derivatives

## Defining the Derivative

#### Tangent Lines

We can obtain the slope of the secant by choosing a value of x near a and drawing a line through the points (a, f(a)) and (x,f(x)). The slope of this line is given by an equation in the form of a difference quotient:
$$
m_{sec} = \frac{(f(x)-f(a))}{x-a}
$$


We can also calculate the slope of a secant line to a function at a value a by using this equation and replacing x with *a + h*, where h is a value close to 0.
$$
m_{sec} = \frac{f(a+h)-f(a)}{h}
$$
The closer the value of a to x the more accurate the slope at point x . Because of this fact we can find the accurate slope at x by finding the limit of f(x) as x approaches a. Let f(x) be a function defined in an open interval containing a. The tangent line to f(x) at a is the line passing through the point (a,f(a)) having slope (provided a limit exists).  
$$
m_{tan} = \lim{x \to a} \frac{(f(x)-f(a))}{x-a}
$$

#### The Derivative of a Function at a Point

The type of limit we compute in order to find the slope of the line tangent to a function is known as the derivative.

 Let f(x) be a function defined in an open interval containing a. The derivative of the function f(x) at a, denoted by f ′(a), is defined by:
$$
f'(a) = \frac{f(a+h)-f(a)}{h}
$$

#### Velocities and Rates of Change

 Recall that if s(t) is the position of an object  moving along a coordinate axis, the average velocity of the object over a time interval [a, t] if t > a or [t, a] if t < a is given by the difference quotient
$$
v_{avg} = \frac{s(t)-s(a)}{t-a}
$$
As the values of t approach a, the values of v_avg approach the value we call the instantaneous velocity at a. That is, instantaneous velocity at a, denoted v(a), is given by:
$$
v(a) = s'(a) = \lim{t \to a} \frac{s(t)-s(a)}{t-a}
$$

## The Derivative as a Function

#### Derivative Functions

Let f be a function. The derivative function, denoted by f ′, is the function whose domain consists of those values  of x such that the following limit exists:
$$
f'(x) = \lim{h \to 0}\frac{f(x+h)-f(h)}{h}
$$
 A function is said to be differentiable on S if it is differentiable at every point in an open set S,
and a differentiable function is one in which f ′(x) exists on its domain.



#### Derivatives and Continuity

Let f(x) be a function and a be in its domain. If f(x) is differentiable at a, then f(x) is continuous at a.  However, if a function is continuous,  however even if a function is continuous it may still fail to be differentiable, for example f(x) = |x| and f(x) = This is because f(x) = |x| turns at a sharp point due to the limit having different values on each side of 0. And f(x) =∛x has a vertical slope at 0.



#### Higher-Order Derivatives

 We can find the derivative of a derivative. These are know as higher order derivatives. 



## Differentiation Rules 

#### The Basic Rules

Let c be a constant. If f(x) = c, then
$$
f'(c) = 0
$$


Let n be a positive integer. If f(x) = x^n, then
$$
f'(x) = nx^{n-1}
$$
The derivative of the sum/difference of a function f and a function g is the same as the sum/difference of the derivative of f and the derivative of g.
$$
\frac{d}{dx}(f(x)\pm g(x)) = \frac{d}{dx}(f(x)) \pm \frac{d}{dx}(g(x))
$$
The derivative of a constant k multiplied by a function f is the same as the constant multiplied  by the derivative:


$$
\frac{d}{dx}(kf(x)) = k\frac{d}{dx}(f(x))
$$

#### Product Rule

Let f(x) and g(x) be differentiable functions. Then 
$$
\frac{d}{dx}(f(x)g(x)) = \frac{d}{dx}f(x)*g(x) +\frac{d}{dx}g(x)*f(x)
$$

#### The Quotient Rule

Let f(x) and g(x) be differentiable functions. Then
$$
\frac{d}{dx}\frac{f(x)}{g(x)} =  \frac{\frac{d}{dx}f(x)*g(x) -\frac{d}{dx}g(x)*f(x)}{g(x)^2}
$$

## Derivatives of Trigonometric Functions

#### Derivatives of the Sine and Cosine Functions

The derivative of the sine function is the cosine and the derivative of the cosine function is the negative sine.
$$
\frac{d}{dx}\sin(x) = \cos(x)
$$

$$
\frac{d}{dx}\cos(x) = -\sin(x)
$$

#### Derivatives of Other Trigonometric Functions

The derivatives of the remaining trigonometric functions are as follows:
$$
\frac{d}{dx} \tan(x) = \sec^2(x)
$$

$$
\frac{d}{dx} \cot(x) = -\csc^2(x)
$$

$$
\frac{d}{dx} \sec(x) = \sec(x)\tan(x)
$$

$$
\frac{d}{dx} \csc(x) = -\csc(x)\cot(x)
$$

#### Higher-Order Derivatives
The higher-order derivatives of sinx and cos x follow a repeating pattern. By following the pattern, we can find any higher-order derivative of sinx and cos x.



## The Chain Rule

#### Deriving the Chain Rule

We can use the chain rule to simplify differentiate composite functions

 Let f and g be functions. For all x in the domain of g for which g is differentiable at x and f is differentiable at g(x), the derivative of the composite function
$$
h(x) = (f ∘g)(x) = f (g(x))
$$


if given by
$$
h'(x) =f'(g(x))g'(x)
$$

#### The Chain and Power Rules Combined

We can also combine the chain rule and power rule to differentiates functions . For all values of x for which the derivative is defined, if
$$
h(x) =(g(x))^n
$$
Then
$$
h'(x) = n(g(x))^{n-1}g'(x)
$$

#### Composites of Three or More Functions

For functions with 3 or more functions we can use the chain rule twice. This looks like:
$$
k'(x) = h'(f(g(x)))f'(g(x))g′(x)
$$

## Derivatives of Inverse Functions

#### The Derivative of an Inverse Function

If f(x) is both invertible and differentiable, the inverse of f(x) is also differentiable. If we recall that  recalling that 
$$
x = f ( f^{-1} (x)))
$$
Then by differntiating this equation we get
$$
1 =f'(f^{-1}(x))(f^{-1}(x)')
$$
Solving for x we get
$$
f^{-1}(x)' = \frac{1}{f'(f^{-1}(x))}
$$

#### Derivatives of Inverse Trigonometric Functions

$$
\frac{d}{dx}\sin^{-1}(x) = \frac{1}{\sqrt{1-(x)^2}}
$$

$$
\frac{d}{dx}\cos^{-1}(x) = \frac{-1}{\sqrt{1-(x)^2}}
$$

$$
\frac{d}{dx}\tan^{-1}(x) = \frac{1}{1+(x)^2}
$$

$$
\frac{d}{dx}\cot^{-1}(x) = \frac{-1}{1+(x)^2}
$$

$$
\frac{d}{dx}\sec ^{-1}(x) = \frac{1}{|x|\sqrt{(x)^2-1}}
$$

$$
\frac{d}{dx}\csc ^{-1}(x) = \frac{-1}{|x|\sqrt{(x)^2-1}}
$$

## Implicit Differentiation

#### Implicit Differentiation

While we normal deal with equation where y is the subjects. We may occasionally need to diferenciate y in terms of x. In these cases we simply differenciate the term and multiple by dy/dx and then factor dy/dx out of these terms. For example
$$
x^2 + y^2 = 25
$$

$$
2x + 2y\frac{dy}{dx} = 0
$$

$$
2y\frac{dy}{dx} = -2x
$$

$$
\frac{dy}{dx} = -\frac{2x}{2y}
$$

$$
\frac{dy}{dx} = -\frac{x}{y}
$$

#### Finding Tangent Lines Implicitly

We can use the technique to find the slope of tangent lines. Take the equation:
$$
y^3 +	x^3 + 3xy = 0
$$
Do find the slope at any point in this line we must differentiate it:
$$
y^3 +	x^3 + 3xy = 0
$$

$$
3y^2 \frac{dy}{dx} +	3x^2 + 3y+\frac{dy}{dx}3x = 0
$$

$$
\frac{dy}{dx}(3y^2 + 3x) + 3x^2 + 3y = 0
$$

$$
\frac{dy}{dx}(3y^2 + 3x) = -(3x^2+3y)
$$

$$
\frac{dy}{dx}= -\frac{(3x^2 +3y)}{(3y^2 + 3x)}
$$

Now we must pick a point we want to find the tangent as. for this example we will use (3/2,3/2)
$$
\frac{dy}{dx}= -\frac{(3(\frac{3}{2})^2 +3(\frac{3}{2}))}{(3(\frac{3}{2})^2 + 3(\frac{3}{2}))}
$$

$$
\frac{dy}{dx} = -1
$$

Then using this value in the slope point equation we get:
$$
y - b = \frac{dy}{dx}(x-a)
$$

$$
y - \frac{3}{2} = -1(x-\frac{3}{2})
$$

$$
y- \frac{3}{2} = -x +  \frac{3}{2}
$$

$$
y = -x +3
$$

## Derivatives of Exponential and Logarithmic Functions

#### Derivative of the Exponential Function

Let E(x) = e^x be the natural exponential function. Then
$$
\frac{d}{dx}(e^{g(x)}) = e^{g(x)}g'(x)
$$

#### Derivative of the Logarithmic Function

If x > 0 and y = ln(x), then
$$
h'(x) = \frac{1}{g(x)}g'(x)
$$
However if we have a logarithm that is of base b we must use the following formula
$$
h'(x) = \frac{g'(x)}{g(x)\ln{b}}
$$
