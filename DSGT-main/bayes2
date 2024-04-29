def bayes_theorem(prior_A, prior_not_A, likelihood_B_given_A, likelihood_B_given_not_A):
    """
    Calculates the posterior probability P(A|B) using Bayes' theorem.

    Parameters:
    prior_A (float): The prior probability of event A, P(A)
    prior_not_A (float): The prior probability of not A, P(not A)
    likelihood_B_given_A (float): The likelihood of event B occurring given A, P(B|A)
    likelihood_B_given_not_A (float): The likelihood of event B occurring given not A, P(B|not A)

    Returns:
    float: The posterior probability of event A occurring, given event B, P(A|B)
    """
    # Calculate the numerator
    numerator = prior_A * likelihood_B_given_A

    # Calculate the denominator
    denominator = (prior_A * likelihood_B_given_A) + (prior_not_A * likelihood_B_given_not_A)

    # Calculate the posterior probability
    posterior_probability = numerator / denominator

    return posterior_probability

# Get user inputs
prior_A = float(input("Enter the prior probability of event A, P(A): "))
prior_not_A = float(input("Enter the prior probability of not A, P(not A): "))
likelihood_B_given_A = float(input("Enter the likelihood of event B occurring given A, P(B|A): "))
likelihood_B_given_not_A = float(input("Enter the likelihood of event B occurring given not A, P(B|not A): "))

# Calculate the posterior probability of A given B, P(A|B)
posterior_probability = bayes_theorem(prior_A, prior_not_A, likelihood_B_given_A, likelihood_B_given_not_A)
print(f"The posterior probability of event A occurring, given event B, P(A|B): {posterior_probability:.4f}")
