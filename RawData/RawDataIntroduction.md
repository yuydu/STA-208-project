Response Varible: Loan Status; Current status of the loan
Predictor Variables: 
['loan_amnt']: the list amount of the loan applied by the borrowers;

['funded_amnt']: the total amount commited to that loan at that point in time;

['funded_amnt_inv']: the total amount commited by investors for that loan at that point in time;

['term']: The number of payments on the loan. 36months/60months;

['int_rate']: interest rate on the loan;

['installment']: the monthly payment owed by the borrower if the loan is ordinates;

*['grade']: LC assigned loan grade;

*['sub_grade']: LC assigned loan subgrade;

*['home_ownership']: The home ownership status provided by the borrower during registration or obtained from the credit report. (RENT, OWN, MORTGAGE, OTHER)

*['annual_inc']: The self-reported annual income provided by the borrower during registration.

['verification_status']: Indicates if income was verified by LC, not verified, or if the income source was verified

['issue_d']: issue date

['purpose']: A category provided by the borrower for the loan request.

??['zip_code']: The first 3 numbers of the zip code provided by the borrower in the loan application.

['addr_state']: The state provided by the borrower in the loan application;

*['delinq_2yrs']: The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years;

['earliest_cr_line']: The month the borrower's earliest reported credit line was opened;

['open_acc']: The number of open credit lines in the borrower's credit file

['revol_bal']: Total credit revolving balance；

['total_acc']: The total number of credit lines currently in the borrower's credit file

(potentional y)['initial_list_status']: The initial listing status of the loan. Possible values are – W, F

['out_prncp']: Remaining outstanding principal for total amount funded; 剩余未偿还本金

['out_prncp_inv']: Remaining outstanding principal for portion of total amount funded by investors；

(?)['total_pymnt']: Payments received to date for total amount funded；

['total_pymnt_inv']: Payments received to date for portion of total amount funded by investors；

['total_rec_prncp']: Principal received to date;

['total_rec_int']: Interest received to date;

['total_rec_late_fee']: 

['recoveries']: post charge off gross recovery;

['collection_recovery_fee']:

['last_pymnt_amnt']:

['last_credit_pull_d']:

['application_type']:

['acc_now_delinq']:

['tot_coll_amt']:

['tot_cur_bal']:

['total_rev_hi_lim']:

['acc_open_past_24mths']:

['avg_cur_bal']:

['chargeoff_within_12_mths']:

['delinq_amnt']:

['mo_sin_old_rev_tl_op']:

['mo_sin_rcnt_rev_tl_op']:

['mo_sin_rcnt_tl']:

['mort_acc']:

['num_accts_ever_120_pd']:

['num_actv_bc_tl']:

['num_actv_rev_tl']:

['num_bc_sats']:

['num_bc_tl']:

['num_il_tl']:

['num_op_rev_tl']:

['num_rev_accts']:

['num_rev_tl_bal_gt_0']:

['num_sats']:

['num_tl_90g_dpd_24m']:

['num_tl_op_past_12m']:

['pct_tl_nvr_dlq']:

['pub_rec_bankruptcies']:

['tax_liens']:

['tot_hi_cred_lim']:

['total_bal_ex_mort']:

['total_bc_limit']:

['total_il_high_credit_limit]:

