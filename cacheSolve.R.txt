cacheSolve <- function(a, ...) {
  k <- a$getInverse()
  if(!is.null(k)){
  message("getting cached data")
  return(k)
  }
  mat <- a$get()
  k <- solve(mat,...)
  a$setInverse(k)
  k
}