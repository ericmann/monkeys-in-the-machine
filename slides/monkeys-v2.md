## Monkeys v2

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

function createNextGeneration() {
    selectParentsForNextGeneration();
    breedNextGeneration();

    if ( theyCanWriteHamlet() ) {
        println( 'done!' );
    } else {
        runAfterTimeout( createNextGeneration, 10 );
    }
}

createNextGeneration();
</code></pre>