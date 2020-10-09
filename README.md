# alternative_hash
Uma criptografia hash alternativa de média complexidade e não descriptografia, chamada atraves da função ahash();
Muito utilizada a hash md5, pensei em alternar e tornar isso um pouco mais complexo, pois na verdade, se trata de uma hash de rápida renderização,
fazendo assim um tempo diminuto pra um ataque de tentativas de chegar a mesma hash de um banco se torne viável.Além de haver possíveis colisões na renderização.

Exemplo 1:

$senha = "123";
$senha = ahash($senha);

echo $senha  ; 
A saida sempre será uma hash de 32bits

/////////////////////////////////////////////////////////////////////////////////////////////////////////

Na função utiliza-se uma hash nativa do php md5(); + reverse + array para string replace.

