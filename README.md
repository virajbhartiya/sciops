<div align="center">

<pre>


███████╗ ██████╗██╗    ██████╗ ██████╗ ███████╗
██╔════╝██╔════╝██║   ██╔═══██╗██╔══██╗██╔════╝
███████╗██║     ██║   ██║   ██║██████╔╝███████╗
╚════██║██║     ██║   ██║   ██║██╔═══╝ ╚════██║
███████║╚██████╗██║   ╚██████╔╝██║     ███████║
╚══════╝ ╚═════╝╚═╝    ╚═════╝ ╚═╝     ╚══════╝
                                            
                                                                                                                                                   

------------------------
Command Line Scientific Calculator. Made with ❤️ using 🦀
</pre>
</div>

## Download

[https://github.com/virajbhartiya/sciops/releases](https://github.com/virajbhartiya/sciops/releases)


## Usage examples

launch the interactive prompt by typing `sciops` to run multiple computations

```sh
a = 10
b = a + 1.14
c = log(b, 3) + sin(PI)
```

or run one off computations by simply providing them

```sh
$ sciops 10 + 1.14
$ sciops '10 + 1.14 * ln(50)'
```

## Features

```sh
# basic arithmetic and assignment
a = 1
b = -2 % a * (3^2 / 4)
b += 100

# functions
               
exp(x)
sqrt(x)
cbrt(x)
abs(x)
floor(x)
ceil(x)
round(x)

ln(x)
log2(x)
log10(x)
log(x, b)

sin(rad)
cos(rad)
tan(rad)

sinh(rad)
cosh(rad)
tanh(rad)

asin(rad)
acos(rad)
atan(rad)

asinh(rad)
acosh(rad)
atanh(rad)
```

All calculations are done using [64 bit *binary* floating point arithmetic](https://en.wikipedia.org/wiki/Double-precision_floating-point_format)
(using the Rust type [`f64`](https://doc.rust-lang.org/std/primitive.f64.html)), so you can come across
the limitations of this implementation, and observe behavior that may be different from other “scientific calculators”, such as the following:
* Rounding errors that may be surprising in decimal notation (e.g. evaluating `0.1 + 0.2` prints `0.30000000000000004`).
* Special values such as “infinity”, “not a number” or a negative zero can be the result of calculations that overflow or have invalid arguments.

## Contributing

1. Fork it (<https://github.com/virajbhartiya/sciops/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request
