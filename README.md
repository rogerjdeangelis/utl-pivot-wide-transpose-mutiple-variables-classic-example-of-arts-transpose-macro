# utl-pivot-wide-transpose-mutiple-variables-classic-example-of-arts-transpose-macro
Pivot wide transpose mutiple variables classic example of arts transpose macro
    %let pgm=utl-pivot-wide-transpose-mutiple-variables-classic-example-of-arts-transpose-macro;

    %stop_submission;

    Pivot wide transpose mutiple variables classic example of arts transpose macro
    A one liner.

    Related repos on end

    github
    https://tinyurl.com/mr9rtttf
    https://communities.sas.com/t5/New-SAS-User/Proc-transpose-to-transform-dataset-from-long-to-wide/m-p/764666#M30499

    /**************************************************************************************************/
    /* INPUT                | PROCESS            | OUTPUT                                             */
    /* =====                | =======            | ======                                             */
    /*   V                T | %utl_transpose(    |     V                T V           T V          T  */
    /*   I                R |  data = have       |     I                R I           R I          R  */
    /*   S                E | ,out  = want       |     S                E S           E S          E  */
    /*   I                A | ,by   = id         |     I                A I           A I          A  */
    /*   T                T | ,var  = visit_num  |     T                T T           T T          T  */
    /*   _     D          M |      diag age      |     _     D          M _   D       M _   D      M  */
    /*   N     I       A  E |      treatment);   |  I  N     I      A   E N   I    A  E N   I    A E  */
    /* I U     A       G  N |                    |  D  U     A      G   N U   A    G  N U   A    G N  */
    /* D M     G       E  T | proc print         |     M     G      E   T M   G    E  T M   G    E T  */
    /*                      |  data=want         |  1  1     1      1   1 2   2    2  2 3   3    3 3  */
    /* 1 1  diabetes  42  1 |  width=min         |  2                                                 */
    /* 2 1  stroke    78  1 |  heading=vertical; |  3  1  diabetes  42  1 .        .  . .        . .  */
    /* 2 2  cancer     .  2 | run;quit;          |     1  stroke    78  1 2 cancer .  2 3 stroke . .  */
    /* 2 3  stroke     .  . |                    |     1  stroke    66  2 2 copd   .  1 3        . .  */
    /* 3 1  stroke    66  2 |                    |                                                    */
    /* 3 2  copd       .  1 |                    |                                                    */
    /* 3 3             .  . |                    |                                                    */
    /*                      |                    |                                                    */
    /* data have;           |                    |                                                    */
    /* input                |                    |                                                    */
    /*    id                |                    |                                                    */
    /*    visit_num         |                    |                                                    */
    /*    diag$             |                    |                                                    */
    /*    age               |                    |                                                    */
    /*    treatment;        |                    |                                                    */
    /* cards4;              |                    |                                                    */
    /* 01 1 diabetes 42 1   |                    |                                                    */
    /* 02 1 stroke 78 1     |                    |                                                    */
    /* 02 2 cancer . 2      |                    |                                                    */
    /* 02 3 stroke . .      |                    |                                                    */
    /* 03 1 stroke 66 2     |                    |                                                    */
    /* 03 2 copd . 1        |                    |                                                    */
    /* 03 3 . . .           |                    |                                                    */
    /* ;;;;                 |                    |                                                    */
    /* run;quit;            |                    |                                                    */
    /*                      |                    |                                                    */
    /**************************************************************************************************/

    REPO
    -------------------------------------------------------------------------------------------------------------------------------------------------
    https://github.com/rogerjdeangelis/utl-transpose-macro-rather-than-proc-print-report-or-tabulate
    https://github.com/rogerjdeangelis/utl-transpose-matrices-with-base-sas
    https://github.com/rogerjdeangelis/utl-transpose-more-than-one-variable
    https://github.com/rogerjdeangelis/utl-transpose-multiple-rows-into-one-row-do_over-dosubl-and-varlist-macros
    https://github.com/rogerjdeangelis/utl-transpose-mutiple-sets-of-variable-fast-macro-transpose
    https://github.com/rogerjdeangelis/utl-transpose-mutiple-variables-with-complete-missing-levels-and-missing-values
    https://github.com/rogerjdeangelis/utl-transpose-pairs-of-dates-by-groups-or-transposing-mutiple-variables
    https://github.com/rogerjdeangelis/utl-transpose-pivot-skinny-to-fat-multiple-sets-of-variables-in-wps-and-sas
    https://github.com/rogerjdeangelis/utl-transpose-pivot-summmarize-in-sql-select-using-r-tidyverse-language-and-sql-sas-r-and-python
    https://github.com/rogerjdeangelis/utl-transpose-pivot-wide-to-long-using-sql-arrays-in-sas-r-and-python
    https://github.com/rogerjdeangelis/utl-transpose-pivot-wide-using-sql-partitioning-in-wps-r-python
    https://github.com/rogerjdeangelis/utl-transpose-sets-of-variables-using-Art-Tabachneck-et-all-very-fast-macro
    https://github.com/rogerjdeangelis/utl-transpose-sets-of-variables-with-a-compound-identification-Arts-macro
    https://github.com/rogerjdeangelis/utl-transpose-successive-sets-of-four-records-in-a-single-column-of-random-numbers-sas-r-sql
    https://github.com/rogerjdeangelis/utl-transpose-table-creating-column-names-from-input-table-rownames-sas-sql-r-pyhon-multi-language
    https://github.com/rogerjdeangelis/utl-transpose-table-with-duplicate-values
    https://github.com/rogerjdeangelis/utl-transposing-a-complex-data-set-in-sas-arts-transpose-macro
    https://github.com/rogerjdeangelis/utl-transposing-and-pivoting-when-id-values-have-duplicates
    https://github.com/rogerjdeangelis/utl-transposing-multiple-variables-using-transpose-macro-sql-arrays-proc-report
    https://github.com/rogerjdeangelis/utl-transposing-normalizing-a-table-using-four-techniques-arrays-untranspose-transpose-and-gather
    https://github.com/rogerjdeangelis/utl-transposing-pivoting-minimums-using-sql-arrays
    https://github.com/rogerjdeangelis/utl-transposing-two-variable-to-columns-using-transpose-macro
    https://github.com/rogerjdeangelis/utl-untranspose-mutiple-arrays-fat-to-skinny-or-normalize
    https://github.com/rogerjdeangelis/utl-using-arts-transpose-macro-with-two-unsorted-tables
    https://github.com/rogerjdeangelis/utl-using-r-to-generate-sql-code-to-pivot-transpose-long-like-sas-array-and-do_over-macros
    https://github.com/rogerjdeangelis/utl-using-sas-gather-macro-to-untranspose-a-fat-dataset-into-one-obsevation
    https://github.com/rogerjdeangelis/utl-very-complex-transpose-with-character-numeric-variables-and-counts-percents
    https://github.com/rogerjdeangelis/utl_an_unsusual_transpose_based_on__groups_of_variable_names
    https://github.com/rogerjdeangelis/utl_classic_transpose_in_r_and_sas
    https://github.com/rogerjdeangelis/utl_diagonal_transpose_while_keeping_all_original_rows
    https://github.com/rogerjdeangelis/utl_excel_Import_and_transpose_range_A9-Y97_using_only_one_procedure
    https://github.com/rogerjdeangelis/utl_flexible_complex_multi-dimensional_transpose_using_one_proc_report
    https://github.com/rogerjdeangelis/utl_simple_three_dimensional_transpose_in_r_and_sas
    https://github.com/rogerjdeangelis/utl_sophisticated_transpose_with_proc_summary_idgroup
    https://github.com/rogerjdeangelis/utl_sort_summarize_and_transpose_multiple_variable_and_create_output_dataset
    https://github.com/rogerjdeangelis/utl_sort_summarize_transpose_and_format_in_1_datastep
    https://github.com/rogerjdeangelis/utl_sort_transpose_and_summarize_a_dataset_using_just_one_proc_report
    https://github.com/rogerjdeangelis/utl_sort_transpose_and_summarize_in_one_proc_v2
    https://github.com/rogerjdeangelis/utl_sort_transpose_summarize
    https://github.com/rogerjdeangelis/utl_sql_version_of_proc_transpose_with_major_advantage_of_summarization
    https://github.com/rogerjdeangelis/utl_techniques_to_transpose_and_stack_multiple_variables
    https://github.com/rogerjdeangelis/utl_transpose_and_concatenate_observations_by_id_in_one_datastep
    https://github.com/rogerjdeangelis/utl_transpose_long_to_wide_with_sequential_matching_pairs
    https://github.com/rogerjdeangelis/utl_transpose_multiple_variables_and_split_variables_into_multiple_variables
    https://github.com/rogerjdeangelis/utl_transpose_rows_to_column_identifying_type_of_data
    https://github.com/rogerjdeangelis/utl_transpose_table_by_two_variables_not_supported_by_proc_transpose
    https://github.com/rogerjdeangelis/utl_transpose_with_multiple_id_values_per_group
    https://github.com/rogerjdeangelis/utl_transpose_with_proc_report
    https://github.com/rogerjdeangelis/utl_transpose_with_proc_sql
    https://github.com/rogerjdeangelis/utl_transposing_multiple_variables_with_different_ids_a_single_transpose_cannot_do_this
    https://github.com/rogerjdeangelis/utl_two_families_itinerary_through_italy_transpose
    https://github.com/rogerjdeangelis/utl_using_a_hash_to_transpose_and_reorder_a_table
    https://github.com/rogerjdeangelis/wps-pivot-longer-transpose--using-r-and-wps-loops


    /*              _
      ___ _ __   __| |
     / _ \ `_ \ / _` |
    |  __/ | | | (_| |
     \___|_| |_|\__,_|

    */

