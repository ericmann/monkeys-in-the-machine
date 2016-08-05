## Monkeys v2

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

while ( ! theyCanWriteHamlet() ) {
    selectParentsForNextGeneration();
    breedNextGeneration();

    // Do something else perhaps?
}

println( 'done!' );
</code></pre>