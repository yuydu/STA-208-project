Response Varible: Loan Status; Current status of the loan
                  
                  dummy: 1, good status: Fully Paid, Current
                         0, bad status: In Grace Period, Late(16-30 days), Late(31-120 days), Default, Charged Off

Predictor Variables: 
['loan_amnt']: the list amount of the loan applied by the borrowers;

['funded_amnt']: the total amount commited to that loan at that point in time;

['funded_amnt_inv']: the total amount commited by investors for that loan at that point in time;

['term']: The number of payments on the loan. 36months/60months;
   
    dummy

['int_rate']: interest rate on the loan;

['installment']: the monthly payment owed by the borrower if the loan is ordinates;

*['grade']: LC assigned loan grade;
      
    delete

*['sub_grade']: LC assigned loan subgrade;

    delete

*['home_ownership']: The home ownership status provided by the borrower during registration or obtained from the credit report. (RENT, OWN, MORTGAGE, OTHER)
  
    dummy

*['annual_inc']: The self-reported annual income provided by the borrower during registration.

['verification_status']: Indicates if income was verified by LC, not verified, or if the income source was verified

    dummy

split training and test ['issue_d']: issue date

['purpose']: A category provided by the borrower for the loan request.--clustering?
  
    dummy estate: car, home-improvement, house, moving, major_purchase, renewable_enery
          money: credit_card, debt_consolidation, small_business
          medical
          vacation, other

??['zip_code']: The first 3 numbers of the zip code provided by the borrower in the loan application.

['addr_state']: The state provided by the borrower in the loan application;

    dummy -- inside/outside state

*['delinq_2yrs']: The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years;

['earliest_cr_line']: The month the borrower's earliest reported credit line was opened;

['open_acc']: The number of open credit lines in the borrower's credit file

['revol_bal']: Total credit revolving balance；

['total_acc']: The total number of credit lines currently in the borrower's credit file

(potentional y)['initial_list_status']: The initial listing status of the loan. Possible values are – W, F
  
    dummy: 1, Whole
           0, Fraction

['out_prncp']: Remaining outstanding principal for total amount funded; 剩余未偿还本金

['out_prncp_inv']: Remaining outstanding principal for portion of total amount funded by investors；

(?)['total_pymnt']: Payments received to date for total amount funded；

['total_pymnt_inv']: Payments received to date for portion of total amount funded by investors；

['total_rec_prncp']: Principal received to date;

['total_rec_int']: Interest received to date;

['total_rec_late_fee']: Late fees received to date;

['recoveries']: post charge off gross recovery  后冲销总回收费用

['collection_recovery_fee']: post charge off collection fee;

['last_pymnt_amnt']: Last total payment amount received;

['last_credit_pull_d']: The most recent month LC pulled credit for this loan;

['application_type']: Indicates whether the loan is an individual application or a joint application with two co-borrowers;

     dummy: 1, individual
            0, joint

['acc_now_delinq']: The number of accounts on which the borrower is now delinquent.

['tot_coll_amt']: Total collection amounts ever owed;

['tot_cur_bal']: Total current balance of all accounts;

['total_rev_hi_lim']: Total revolving high credit/credit limit;

['acc_open_past_24mths']: Number of trades opened in past 24 months.;

['avg_cur_bal']: Average current balance of all accounts;

['chargeoff_within_12_mths']: Number of charge-offs within 12 months;

['delinq_amnt']: The past-due amount owed for the accounts on which the borrower is now delinquent;

['mo_sin_old_rev_tl_op']: Months since oldest revolving account opened;

['mo_sin_rcnt_rev_tl_op']: Months since most recent revolving account opened;

['mo_sin_rcnt_tl']: Months since most recent account opened;

['mort_acc']: Number of mortgage accounts.

['num_accts_ever_120_pd']: Number of accounts ever 120 or more days past due;

['num_actv_bc_tl']: Number of currently active bankcard accounts;

['num_actv_rev_tl']: Number of currently active revolving trades;

['num_bc_sats']: Number of satisfactory bankcard accounts;

['num_bc_tl']: Number of bankcard accounts;

['num_il_tl']: Number of installment accounts;

['num_op_rev_tl']: Number of open revolving accounts;

['num_rev_accts']: Number of revolving accounts;

['num_rev_tl_bal_gt_0']: Number of revolving trades with balance >0;

['num_sats']: Number of satisfactory accounts;

['num_tl_90g_dpd_24m']: Number of accounts opened in past 24 months;

['num_tl_op_past_12m']: Number of accounts opened in past 12 months;

['pct_tl_nvr_dlq']: Percent of trades never delinquent;

['pub_rec_bankruptcies']: Number of public record bankruptcies;

['tax_liens']: Number of tax liens;

['tot_hi_cred_lim']: Total high credit/credit limit;

['total_bal_ex_mort']: Total credit balance excluding mortgage;

['total_bc_limit']: Total bankcard high credit/credit limit;

['total_il_high_credit_limit]: Total installment high credit/credit limit.

