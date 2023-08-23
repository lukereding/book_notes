## Managing model risk
Broucke and Baesens

There were some interesting ideas in this book, overall I find it's usefulness largely limited to the some of structure and articulation of _types_ of model risk that exist.

The book breaks down model risk into components based on the machine learning delivery lifecycle, CRISP-DM, KDD, or whatever you want to call it:

### data risk

- bias in data
  - exogenous factors
  - company strategy at the time of build sample
  - inappropriate data
- data perimeter or sample characteristics
  - e.g., building on a different sample than you score on
- data quality. there's a pretty interesting taxonomy here
  - intrinsic
    - accurate
    - objective
    - reputation
  - contextual
    - completeness
    - appropriate amount
    - value added
    - releance
    - timeliness
    - actionable
  - representation
    - interpretable
    - understandable
    - consistent
    - concisely-represented
    - alighment
  - access
    - accessible
    - secure
    - traceable
- lack of predictive power
- data regulation risk
- not enough data
- incomplete or noisy labels

### specification risk

- basically, you botch the target variable definition in some way
- there's some interesting stuff in here about customer lifetime value modeling
- the target variable often contains a lot of hidden assumptions and shortcuts, and extra care should be paid to it
- wrong loss function
- multicollinearity between predictors

### development risk

- domain knowledge paradox
  - i.e., you want a model that makes sense
  - but if you knew everything the model did, you wouldn't need a model
- citizen data science risk
  - i.e., people building models using auto-ml and related tools without really understanding what they're doing
- data leakage
- technological myopia
- programming errors
- meaningful violation of important assumptions
- documentation risk
- losing the end users
  - i.e., not keeping the people who are going to be using the model informed and in-the-loop
- vendor lock in
- risks of open source
  - some interesting perspectives in here, especially around the true costs of using OSS
  - a lot of it boils down to: use common sense and a basic risk assessment when choosing your tools

### validation risk

-

### operational risk

### security risk


### managerial risk


### other

Good qualities for a predictive model:

- valid
- useful
- unexpected
- understandable

Drivetrain approach to model development:

1. define the objective
2. determine the levers of control
3. determine the data that can be collected
4. model construction

Look into Bayesian networks

