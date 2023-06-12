great job!
for returning the average even when some of the movies don't have a score, you need to check if the score property (curr.score) exists, and if it doesn't just return the acc

  const totalScore = moviesArray.reduce((acc , curr) => {
   if (!curr.score) return acc;
   return acc + curr.score
  }, 0);
