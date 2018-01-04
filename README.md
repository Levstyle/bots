# bots

## Документы:
1. [Research results](https://docs.google.com/document/d/1CLdp-yWtlK5PDOpZGZG-pR-jZBC11tm5csjfA3HQUDE/edit?usp=sharing)
(много полезных ссылок в разделе "Материалы")
## Репозитории:
1. [Hybrid code networks, End-To-End Dialog System](https://github.com/chagge/n2n_dialog_system) | [исправленный в соответствии с актуальний версией tensorflow код](n2n_dialog_system)
2. [The implementation of key value memory networks in tensorflow](https://github.com/siyuanzhao/key-value-memory-networks) | [исправленный в соответствии с актуальний версией tensorflow код](key-value-memory-networks)
3. [Keras DL models to answer 8th grade science multiple choice questions](https://github.com/sujitpal/dl-models-for-qa)

4. [Simple ChatBot introducing NLP and Machine Learning for Classification of Sentences](https://github.com/edbullen/NLPBot)
5. [tensorflow implementation of "A neural conversational model", a Deep learning based chatbot](https://github.com/Conchylicultor/DeepQA)

## Warning:
В новых версиях tensorflow в некоторых функциях сломана обратная совместимость. В основном правки в коде с репозиториев #1, #2 связаны с этим.

На версиях tensorflow<1.0 код с репозиториев #1, #2 должен работать без модификаций.

Примеры:

`tf.op_scope` -> `tf.name_scope` (+ изменен порядок аргументов)

`tf.concat` (изменен порядок аргументов)

`tf.split` (изменен порядок аргументов)

`tf.nn.bidirectional_rnn` -> `tf.contrib.rnn.static_bidirectional_rnn`

`tf.nn.rnn` -> `tf.nn.static_rnn`

`tf.mul` -> `tf.multiply`
