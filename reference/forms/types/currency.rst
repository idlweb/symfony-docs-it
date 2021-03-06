.. index::
    single: Form; Campi; currency

Tipo di campo currency
======================

Il tipo ``currency`` è un sottoinsieme del
:doc:`campo choice </reference/forms/types/choice>` che permette all'utente
di selezionare da una grande lista di valute `ISO 4217 a 3 lettere`_.

A differenza del tipo ``choice``, non c'è bisogno di specificare le opzioni
``choices`` o ``choice_list`` dato che il campo usa automaticamente una grande lista di
valute. *È possibile* anche specificare queste opzioni manualmente, ma in questo caso
si dovrebbe usare il tipo ``choice`` direttamente.

+---------------+------------------------------------------------------------------------+
| Reso come     | possono essere vari tag (vedi :ref:`forms-reference-choice-tags`)      |
+---------------+------------------------------------------------------------------------+
| Opzioni       | - `choices`_                                                           |
| Sovrascritte  |                                                                        |
+---------------+------------------------------------------------------------------------+
| Opzioni       | - `multiple`_                                                          |
| ereditate     | - `expanded`_                                                          |
|               | - `preferred_choices`_                                                 |
|               | - `empty_value`_                                                       |
|               | - `error_bubbling`_                                                    |
|               | - `empty_data`_                                                        |
|               | - `required`_                                                          |
|               | - `label`_                                                             |
|               | - `label_attr`_                                                        |
|               | - `data`_                                                              |
|               | - `read_only`_                                                         |
|               | - `disabled`_                                                          |
|               | - `mapped`_                                                            |
+---------------+------------------------------------------------------------------------+
| Tipo genitore | :doc:`choice </reference/forms/types/choice>`                          |
+---------------+------------------------------------------------------------------------+
| Classe        | :class:`Symfony\\Component\\Form\\Extension\\Core\\Type\\CurrencyType` |
+---------------+------------------------------------------------------------------------+

Opzioni ridefinite
------------------

choices
~~~~~~~

**default**: ``Symfony\Component\Intl\Intl::getCurrencyBundle()->getCurrencyNames()``

L'opzione choices è impostata di default a tutte le valute.

Opzioni ereditate
-----------------

Queste opzioni sono eredidate dal tipo :doc:`choice </reference/forms/types/choice>`:

.. include:: /reference/forms/types/options/multiple.rst.inc

.. include:: /reference/forms/types/options/expanded.rst.inc

.. include:: /reference/forms/types/options/preferred_choices.rst.inc

.. include:: /reference/forms/types/options/empty_value.rst.inc

.. include:: /reference/forms/types/options/error_bubbling.rst.inc

Queste opzioni sono eredidate dal tipo :doc:`form </reference/forms/types/form>`:

.. include:: /reference/forms/types/options/empty_data.rst.inc

.. include:: /reference/forms/types/options/required.rst.inc

.. include:: /reference/forms/types/options/label.rst.inc

.. include:: /reference/forms/types/options/label_attr.rst.inc

.. include:: /reference/forms/types/options/data.rst.inc

.. include:: /reference/forms/types/options/read_only.rst.inc

.. include:: /reference/forms/types/options/disabled.rst.inc

.. include:: /reference/forms/types/options/mapped.rst.inc

.. _`ISO 4217 a 3 lettere`: http://en.wikipedia.org/wiki/ISO_4217
