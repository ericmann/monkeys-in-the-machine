## Monkeys v2

<pre><code data-trim lang="javascript">
createRandomPopulation();

function breedMonkeys()
{
    selectParentsForNextGeneration();
    yield breedNextGeneration();
}

while ( bestFitness() !== 0 ) {
	breedMonkeys();

    // Do something else perhaps?
}

println( 'done!' );
</code></pre>