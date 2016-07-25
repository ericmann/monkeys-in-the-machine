## Monkeys v3

<pre class="fragment"><code data-trim lang="javascript">
(function() {
    createRandomPopulation();

    for ( var worker in workers ) {
        worker.postMessage( JSON.stringify( { 'method': 'breedNext' } ) );
    }

    $.when.apply( $, workers ).then( function() {
        alert( 'done' );
    } );
})();
</code></pre>