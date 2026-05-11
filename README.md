
# USER CONFIGURATION (edit these for your own dataset)

CSV_PATH      = "your_dataset.csv"       # path to your CSV file 

TARGET_COL    = "cancer"                 # name of your binary label column (0/1)

FEATURE_COLS  = ["feat1", "feat2", ...]  # list of your numeric feature columns

RANDOM_STATE  = 42                       # for reproducibility

TEST_SIZE     = 0.2                      # held-out split fraction

N_SYNTH       = 300                      # how many synthetic samples to generate

BLEND         = 0.4                      # VAE fraction (0.4 gave best F1 here for MammoWave)

MARGIN        = 0.20                     # boundary filter tolerance


# Load your dataset
clean_df = pd.read_csv(CSV_PATH)
