# loss
function computeLoss(costPrice, sellingPrice) {
    /**
     * This function computes the loss incurred based on the cost price and selling price of a product.
     * 
     * @param {number} costPrice - The cost price of the product.
     * @param {number} sellingPrice - The selling price of the product.
     * @returns {number} The loss incurred.
     */
    
    try {
        // Check if both arguments are numbers
        if (typeof costPrice !== 'number' || typeof sellingPrice !== 'number') {
            throw new TypeError('Both arguments must be numbers');
        }
        
        // Calculate the loss
        const loss = costPrice - sellingPrice;
        
        // Return the loss
        return loss;
    } catch (error) {
        // Log the error
        console.error(`Error: ${error.message}`);
        return 0;
    }
}
