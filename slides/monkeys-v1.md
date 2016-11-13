## Monkeys v1

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

while ( bestFitness() !== 0 ) {
    breedNextGeneration();
}

println( 'done!' );
</code></pre>