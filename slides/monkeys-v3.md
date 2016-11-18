## Monkeys v3

<pre class="fragment"><code data-trim lang="javascript">
createRandomPopulation();

$collectors = [];
foreach( $threads as $thread ) {
	array_push( $collectors, runInThread( $thread, 'breedSome' ) );
}

$once = breedSome();

foreach( $threads as $thread ) {
    $once = array_merge( $once, $thread->result() );
}

println( 'done!' );
</code></pre>
