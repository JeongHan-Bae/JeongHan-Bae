# 👋 Hi, I'm [@JeongHan-Bae](https://github.com/JeongHan-Bae)

🎯 **Software Development Project Manager** | **Technical Leadership & Architecture Background**  
🧩 Managing cross-functional engineering teams with a foundation in **C++** and **Python**

---

## 🚀 About Me

- 🧱 Building **maintainable, auditable, production-grade systems**
- 🧠 Writing **modern C++** and **Python** with discipline, not decoration  
- 🔎 Prioritizing **clarity, traceability, and operational stability**
- ⚓️ Grounding software in **real business constraints and measurable impact**
- 🏝 Starting from **essential MVPs**, expanding only when real requirements demand it  

💬 *"No over-engineering. No unnecessary abstraction. Just solid systems that work."*

## Visual Tech Stack

> **Note:**
> 
> Only core technologies aligned with my engineering philosophy are displayed in the icon stack.
> 
> When a primary technology does not have an available icon on https://skillicons.dev/,
> for example **Boost**, it is not shown despite being strongly endorsed.
>
> <p align="center">
>   <img src="https://upload.wikimedia.org/wikipedia/commons/b/be/Boost.svg"
>        width="70"
>        alt="Boost Logo" />
> </p>
>
> When a technology does have an available icon on https://skillicons.dev/,
> for example **Qt**, but does not align with my core engineering direction, it is intentionally not displayed.
>
> <p align="center">
>   <img src="https://skillicons.dev/icons?i=qt"
>        width="70"
>        alt="Qt Icon" />
> </p>

The following represents the core technology stack:

<!-- C++ Ecosystem -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=cpp,cmake,opencv&theme=light" />
</p>

<!-- Python Ecosystem -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=python,fastapi,django&theme=dark" />
</p>

<!-- Java Ecosystem -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=java,spring,maven,gradle&theme=light" />
</p>

<!-- Web Frontend -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=ts,vite,vue&theme=dark" />
</p>

<!-- CI & Testing -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=github,githubactions,jenkins,selenium&theme=light" />
</p>

<!-- Databases -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=mysql,postgresql,sqlite&theme=dark" />
</p>

<!-- DevOps -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=docker,kubernetes,git&theme=light" />
</p>

<!-- Systems / IDE -->
<p align="center">
  <img src="https://skillicons.dev/icons?i=linux,ubuntu,debian,apple,vscode,idea&theme=light" />
</p>

Although I’m capable of working with several native frontend environments, I intentionally avoid using many of them.  
I prefer building frontend applications on the web — especially with Vite + Vue 3.  
If possible, I favor RESTful architecture (while being fully proficient in gRPC), 
simply because I prefer the clarity and simplicity of REST.

## 📈 GitHub Contribution Snake

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/JeongHan-Bae/JeongHan-Bae/output/github-contribution-grid-snake-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/JeongHan-Bae/JeongHan-Bae/output/github-contribution-grid-snake.svg">
  <img alt="GitHub Snake Animation" src="https://raw.githubusercontent.com/JeongHan-Bae/JeongHan-Bae/output/github-contribution-grid-snake.svg">
</picture>

---

## 📫 How to Reach Me

📧 [mastropseudo@gmail.com](mailto:mastropseudo@gmail.com)

Let's connect and turn ambitious ideas into **well-structured, deliverable projects**.

## A Quiet Sign-Off

If you’ve reached this far,  
thank you for walking through these lines of code and thought.

Before the page ends, I’ll leave a small Tcl script —  
a gentle farewell written in the language I enjoy.

Here is a playful, lightly obfuscated fragment — 
a small tribute to my Grande École geek years, before I became the serious engineer I am today.

<details>
<summary>One last script</summary>

```tcl
#!/usr/bin/env tclsh

proc fastpow {base exp} {
    if {$exp < 0} {
        error "Negative exponent not supported"
    }

    set result 1
    set b $base
    set e $exp

    while {$e > 0} {
        if {$e % 2 == 1} {
            set result [expr {$result * $b}]
        }
        set b [expr {$b * $b}]
        set e [expr {$e / 2}]
    }

    return $result
}

proc f {x} {
    expr {
        (
            5449249 * [fastpow $x 4]
            - 1775640448 * [fastpow $x 3]
            + 192283248169 * [fastpow $x 2]
            - 6920941047270 * $x
            + 389518044300
        )
        / 3856614300
    }
}

proc g {x} {
    expr {
        (
            444011 * [fastpow $x 3]
            - 85822707 * [fastpow $x 2]
            + 3965440996 * $x
            + 18632136600
        )
        / 282305100
    }
}

proc generate_code {x0} {
    set x $x0
    set code ""

    while {1} {
        set y [f $x]

        if {$y < 0} {
            break
        }

        append code [format %c $y]
        set x $y
    } ;# 101 120 105 116 -1

    return $code
}

proc generate_str {x0} {
    set x $x0
    set str ""
    set iter 0

    while {1} {
        incr iter
        set y [g $x]

        if {$y == $iter} {
            break
        }

        append str [format %c $y]
        set x $y
    } ;# 66 121 101 4

    return $str
}

proc _hook {cmd op} {
    puts [generate_str 0]
}

trace add execution [generate_code 0] enter _hook

apply [list {} [generate_code 0]]
```

</details>
