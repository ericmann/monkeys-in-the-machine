## Monkeys v3

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

foreach( $threads in $thread ) {
	runInThread( $thread, breedNextGeneration );
}

when( $threads )->then( function() {
    println( 'done!' );
} );
</code></pre>