## Monkeys v2

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

while ( bestFitness() !== 0 ) {
    breedNextGeneration();

    // Do something else perhaps?
}

println( 'done!' );
</code></pre>