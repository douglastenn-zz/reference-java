## Streams e Parallel Streams

A nova funcionalidade que foi adicionado ao java 8 são as streams.
Stream é nada mais que uma forma diferente de criar um elemento, seja esse elemento uma collection, array ou outra coisa. Por padrão o java implementa uma interface de `Collection` para o elemento que é aplicado.
Com um elemento stream, podemos utilizar diversas operações como: distinct, count, map, filter, reduce, allMatch, noneMatch, etc.

A principal diferença entre stream e parallelStream é a sua forma de processamento, stream utiliza `single threading` enquanto parallelStream utiliza `multi threading`, e seu processamento é em paralelo utilizando multi cores do processador.

