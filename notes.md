# Variables

- the host platform (hardware and operating system)
- the language
- runtime (compiler and associated libraries)
- the heap size
- the nondeterminism
- warm-up of the runtime system

## Control Non-determinism

Over time, we have adopted and recommend three different strategies: (a) use
deterministic replay of optimization plans, which requires JVM support, (b) take
multiple measurements in a single JVM invocation, after reaching steady state
and turning off the JIT compiler, and (c) generate sufficient data points and
apply suitable statistical analysis.

# Metrics

 - dynamic heap composition graphs, which measure time-varying lifetime
   properties of the heap
 - architectural characteristics such as branch misprediction rates and
   instruction mix

# Quotes

> Garbage collection is fundamentally a space- time tradeoff between the
> efficacy of space reclamation and time spent reclaiming objects; heap size is
> the key control variable. The smaller the heap size, the more often the
> garbage collector will be invoked and the more work it will perform.

              - Wake Up and Smell the Coffee: Evaluation Methodology for the
                21st Century

> Sound methodology includes using appropriate workloads, principled
> experimental design, and rigorous analysis.

              - Wake Up and Smell the Coffee: Evaluation Methodology for the
                21st Century


# Pick non trivial app :

  - Multi-threaded
  - Rails ?
  - Sinatra ?
  - Other (Pure) Ruby Project ? (Top Github ?)
    - [defunk/mustache](https://github.com/defunkt/mustache)

# Inspirational Projects

 - DaCapo Benchmarks
