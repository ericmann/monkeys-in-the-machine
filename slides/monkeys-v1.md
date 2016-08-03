## Monkeys v1

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

selectParentsForNextGeneration();
breedNextGeneration();

if ( theyCanWriteHamlet() ) {
    println( 'done!' );
} else {
    selectParentsForNextGeneration();
    breedNextGeneration();

    // ... iterate 5000+ times
}
</code></pre>