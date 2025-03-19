
app.post('/api/teams/:team_id/investments', (req, res) => {
  const { investmentAmount, planId } = req.body;

  if (investmentAmount < 10) {
    return res.status(400).json({ error: "Minimum investment is $10." });
  }

  // Proceed with the investment logic here...
});
