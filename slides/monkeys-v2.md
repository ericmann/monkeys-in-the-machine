## Monkeys v2

<pre class="fragment"><code data-trim lang="javascript">
(function() {
    createRandomPopulation();

    function createNextGeneration() {
        selectParentsForNextGeneration();
        breedNextGeneration();

        if ( theyCanWriteHamlet() ) {
            alert( 'done!' );
        } else {
            window.setTimeout( createNextGeneration, 10 );
        }
    }

    createNextGeneration();
})();
</code></pre>