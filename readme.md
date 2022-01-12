<!-- antes de enviar a versão final, solicitamos que todos os comentários, colocados para orientação ao aluno, sejam removidos do arquivo -->
# Análise de Sentimentos  Comparando a Acurácia na Utilzação do NLTK e AFINN e A Análise de Emoções Utilizando o TEXT2EMOTION

#### Aluno: [Fábio Mendonça dos Santos](https://github.com/link_do_github)
#### Orientador: [Leonardo Alfredo Forero Mendonza](https://github.com/link_do_github) .

---

Trabalho apresentado ao curso [BI MASTER](https://ica.puc-rio.ai/bi-master) como pré-requisito para conclusão de curso e obtenção de crédito na disciplina "Projetos de Sistemas Inteligentes de Apoio à Decisão".


- Link para os códigos. 
- [tcc_fabio_tweets_filter_retweets.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_filter_retweets.ipynb)
- [tcc_fabio_tweets_concat_csv.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_concat_csv.ipynb)
- [tcc_fabio_tweets_classificação_sentimentos_emoções.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_classifica%C3%A7%C3%A3o_sentimentos_emo%C3%A7%C3%B5es.ipynb)
- [tcc_fabio_tweets_emoções_cnn_lstmvf.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_emo%C3%A7%C3%B5es_cnn_lstmvf.ipynb)
- [tcc_fabio_tweets_sentimentos_affin_class_cnn_lstmvf.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_sentimentos_affin_class_cnn_lstmvf.ipynb)
- [tcc_fabio_tweets_sentimentos_nltk_class_cnn_lstmvf.ipynb](https://github.com/fmansantos/TCC-BI-MASTER/blob/main/tcc_fabio_tweets_sentimentos_nltk_class_cnn_lstmvf.ipynb)

- [Link para a monografia](https://link_da_monografia.com). <!-- caso não aplicável, remover esta linha -->


---

### Resumo



Este trabalho buscou explorar o processo BI desde a obtenção da informação que neste caso são tweets que foram extraídos diariamente 15.000 por dia, filtrando o retweets.
Após e extração os arquivos foram concatenados em um único arquivo com 210.303 registros.
Este arquivo único foi analisado e teve os sentimentos  e emoções classificados.
Para a análise de sentimentos foram utilizados o NLTK e o AFINN, para a análise de emoções foi utilizado o TEXT2EMOTION,com as classficações gravadas em arquivos para análise psterior.  
Após a classificação dos sentimentos e emoções, foram aplicados os pré-processamentos para retirar o que não serve para as análises de sentimentos e emoções feitas com a utilização de redes neurias.


### Abstract <!-- Opcional! Caso não aplicável, remover esta seção -->

<!-- trocar o texto abaixo pelo resumo do trabalho, em inglês -->

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

Donec molestie, ante quis tempus consequat, mauris ante fringilla elit, euismod hendrerit leo erat et felis. Mauris faucibus odio est, non sagittis urna maximus ut. Suspendisse blandit ligula pellentesque tincidunt malesuada. Sed at ornare ligula, et aliquam dui. Cras a lectus id turpis accumsan pellentesque ut eget metus. Pellentesque rhoncus pellentesque est et viverra. Pellentesque non risus velit. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.

### 1. Introdução

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 2. Modelagem

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 3. Resultados

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

### 4. Conclusões

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin pulvinar nisl vestibulum tortor fringilla, eget imperdiet neque condimentum. Proin vitae augue in nulla vehicula porttitor sit amet quis sapien. Nam rutrum mollis ligula, et semper justo maximus accumsan. Integer scelerisque egestas arcu, ac laoreet odio aliquet at. Sed sed bibendum dolor. Vestibulum commodo sodales erat, ut placerat nulla vulputate eu. In hac habitasse platea dictumst. Cras interdum bibendum sapien a vehicula.

Proin feugiat nulla sem. Phasellus consequat tellus a ex aliquet, quis convallis turpis blandit. Quisque auctor condimentum justo vitae pulvinar. Donec in dictum purus. Vivamus vitae aliquam ligula, at suscipit ipsum. Quisque in dolor auctor tortor facilisis maximus. Donec dapibus leo sed tincidunt aliquam.

---

Matrícula: 201.190.260

Pontifícia Universidade Católica do Rio de Janeiro

Curso de Pós Graduação *Business Intelligence Master*
