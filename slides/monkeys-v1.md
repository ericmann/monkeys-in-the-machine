## Monkeys v1

<pre class="fragment"><code data-trim lang="javascript">
(function() {
    createRandomPopulation();

    selectParentsForNextGeneration();
    breedNextGeneration();

    if ( theyCanWriteHamlet() ) {
        alert( 'done!' );
    } else {
        selectParentsForNextGeneration();
        breedNextGeneration();

        // ... iterate 5000+ times
    }
})();
</code></pre>