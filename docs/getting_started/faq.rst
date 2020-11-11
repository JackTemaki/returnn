.. _faq.rst:

==========================
Frequently Asked Questions
==========================


How can I update to Tensorflow 2?
---------------------------------

RETURNN can run any config with both Tensorflow 1 and Tensorflow 2 in graph mode.
The code for handling the correct imports is :class:`returnn.tf.compat`.
If you have custom code in your config that uses :code:`import tensorflow as tf`
you may experience missing functions or changed behaviour.
In this case, replace the imports by :code:`from returnn.tf.compat import v1 as tf`
If you experience any other issues after changing to Tensorflow 2, please open an issue.




