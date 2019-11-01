<template>
	<div class="container">
		<div class="row">
			<div class="col">		
				<h2 class="py-4">Typography</h2>
				<table class="table">
					<tbody>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h1&gt;&lt;/h1&gt;</code></p>
						</td>
						<td><span class="h1">h1. Bootstrap heading</span></td>
						</tr>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h2&gt;&lt;/h2&gt;</code></p>
						</td>
						<td><span class="h2">h2. Bootstrap heading</span></td>
						</tr>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h3&gt;&lt;/h3&gt;</code></p>
						</td>
						<td><span class="h3">h3. Bootstrap heading</span></td>
						</tr>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h4&gt;&lt;/h4&gt;</code></p>
						</td>
						<td><span class="h4">h4. Bootstrap heading</span></td>
						</tr>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h5&gt;&lt;/h5&gt;</code></p>
						</td>
						<td><span class="h5">h5. Bootstrap heading</span></td>
						</tr>
						<tr>
						<td>
							<p><code class="highlighter-rouge">&lt;h6&gt;&lt;/h6&gt;</code></p>
						</td>
						<td><span class="h6">h6. Bootstrap heading</span></td>
						</tr>
					</tbody>
					</table>
			</div>
		</div>
		<div class="row">
			<div class="col">
				<h2 class="py-3">Paragraph</h2>
				<p>ABCDEFGHIJKLMNOPQRSTUVWXYZ abcdefghijklmnopqrstuvwxyz 0123456789 éáűőúöüóí ÉÁŰŐÚÖÜÓÍ</p>
				<p>An example paragraph with <strong>strong text</strong> and <em>emphasized text</em>, spanning <br/>multiple lines so you can see the line-height.</p>
				<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec varius ipsum tortor, eget convallis ante sagittis ac. Nulla eget bibendum dolor. Praesent at ipsum bibendum, malesuada quam tincidunt, lobortis purus. Donec vel mi mollis,
					sagittis libero non, ultrices elit. Nulla non mauris in sapien mattis scelerisque. Vivamus maximus tincidunt mi, interdum pellentesque urna feugiat sed. Suspendisse vulputate metus leo, nec hendrerit sapien tincidunt ac. Vivamus
					non libero luctus, suscipit libero ut, elementum enim. <a class="link" href="#">Read more</a></p>
				<p>Fusce aliquam sem lorem, in porttitor orci dignissim at. Sed non dolor at orci dignissim bibendum a non nibh. Duis nec vestibulum dui, sit amet lobortis ligula. Sed aliquam mauris nunc, eu sodales est faucibus vitae. Ut sed accumsan
					lectus. Interdum et <a class="link" href="#">malesuada</a> fames ac ante ipsum primis in faucibus. Aenean dignissim odio vehicula ligula varius, ac ullamcorper tortor molestie. Phasellus dolor dui, egestas id ornare in, suscipit
					et dolor.</p>	
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h2 class="py-3">Buttons</h2>
				<fieldset>
						<legend>Normal buttons</legend>
						<button type="button" class="btn btn-primary">Primary</button>
						<button type="button" class="btn btn-secondary">Secondary</button>
						<button type="button" class="btn btn-success">Success</button>
						<button type="button" class="btn btn-danger">Danger</button>
						<button type="button" class="btn btn-warning">Warning</button>
						<button type="button" class="btn btn-info">Info</button>
						<button type="button" class="btn btn-light">Light</button>
						<button type="button" class="btn btn-dark">Dark</button>

						<button class="btn btn-primary">
							<span class="spinner-border spinner-border-sm"></span>
						</button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<fieldset>
					<legend>Large buttons</legend>
					<button type="button" class="btn btn-primary btn-lg">Primary</button>
					<button type="button" class="btn btn-secondary btn-lg">Secondary</button>
					<button type="button" class="btn btn-success btn-lg">Success</button>
					<button type="button" class="btn btn-danger btn-lg">Danger</button>
					<button type="button" class="btn btn-warning btn-lg">Warning</button>
					<button type="button" class="btn btn-info btn-lg">Info</button>
					<button type="button" class="btn btn-light btn-lg">Light</button>
					<button type="button" class="btn btn-dark btn-lg">Dark</button>	

					<button class="btn btn-primary btn-lg">
						<span class="spinner-border spinner-border-sm"></span>
					</button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<fieldset>
					<legend>Small buttons</legend>
					<button type="button" class="btn btn-primary btn-sm">Primary</button>
					<button type="button" class="btn btn-secondary btn-sm">Secondary</button>
					<button type="button" class="btn btn-success btn-sm">Success</button>
					<button type="button" class="btn btn-danger btn-sm">Danger</button>
					<button type="button" class="btn btn-warning btn-sm">Warning</button>
					<button type="button" class="btn btn-info btn-sm">Info</button>
					<button type="button" class="btn btn-light btn-sm">Light</button>
					<button type="button" class="btn btn-dark btn-sm">Dark</button>	

					<button class="btn btn-primary btn-sm">
						<span class="spinner-border spinner-border-sm"></span>
					</button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<fieldset>
					<legend>Disabled buttons</legend>
					<button type="button" class="btn btn-primary btn" disabled>Primary</button>
					<button type="button" class="btn btn-secondary btn" disabled>Secondary</button>
					<button type="button" class="btn btn-success btn" disabled>Success</button>
					<button type="button" class="btn btn-danger btn" disabled>Danger</button>
					<button type="button" class="btn btn-warning btn" disabled>Warning</button>
					<button type="button" class="btn btn-info btn" disabled>Info</button>
					<button type="button" class="btn btn-light btn" disabled>Light</button>
					<button type="button" class="btn btn-dark btn" disabled>Dark</button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<fieldset>
					<legend>Icon buttons</legend>
					<button class="btn btn-danger"><i class="fas fas fa-trash-alt fa-lg"></i> Delete</button>
					<button class="btn btn-success"><i class="fas fas fa-pencil-alt fa-lg"></i> Edit</button>
					<button class="btn btn-primary"><i class="fas fa-home fa-lg"></i> Home</button>
					<button class="btn btn-info"><i class="fas fa-tasks fa-lg"></i> Tasks</button>
					<button class="btn btn-light"><i class="fas fa-comments fa-lg"></i> Chat</button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<fieldset>
					<legend>Floating buttons</legend>
						<button class="btn btn-success" style="border-radius:50%"><i class="fas fa-plus"></i></button>
						<button class="btn btn-danger" style="border-radius:50%"><i class="fas fa-trash"></i></button>
						<button class="btn btn-info" style="border-radius:50%"><i class="fas fa-bars"></i></button>
						<button	class="btn btn-primary" style="border-radius:50%" disabled><i class="fas fa-comment"></i></button>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h2 class="py-3">Form elements</h2>
				<form action="#">
					<fieldset>
						<legend>Input fields</legend>
						<div class="form-group">
							<label for="exampleFormControlInput1">Email address</label>
							<input type="email" class="form-control" id="exampleFormControlInput1" placeholder="name@example.com">
						</div>
						<div class="form-group">
							<label for="exampleFormControlTextarea1">Example textarea</label>
							<textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
						</div>
					</fieldset>
					<fieldset>
						<legend>Selections</legend>
						<div class="form-group">
							<label for="exampleFormControlSelect1">Example select</label>
							<select class="form-control" id="exampleFormControlSelect1">
							<option>1</option>
							<option>2</option>
							<option>3</option>
							<option>4</option>
							<option>5</option>
							</select>
						</div>
						<div class="form-group">
							<label for="exampleFormControlSelect2">Example multiple select</label>
							<select multiple class="form-control" id="exampleFormControlSelect2">
							<option>1</option>
							<option>2</option>
							<option>3</option>
							<option>4</option>
							<option>5</option>
							</select>
						</div>
						<div>
							<label for="inputPassword5">Password</label>
							<input type="password" id="inputPassword5" class="form-control" aria-describedby="passwordHelpBlock">
							<small id="passwordHelpBlock" class="form-text text-muted">
							Your password must be 8-20 characters long, contain letters and numbers, and must not contain spaces, special characters, or emoji.
							</small>
						</div>
					</fieldset>
				</form>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<form action="#">
					<fieldset>
						<legend>Radio buttons</legend>
						<div class="form-check">
							<input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios1" value="option1" checked>
							<label class="form-check-label" for="exampleRadios1">
								Default radio
							</label>
							</div>
							<div class="form-check">
								<input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios2" value="option2">
								<label class="form-check-label" for="exampleRadios2">
									Second default radio
								</label>
							</div>
							<div class="form-check disabled">
								<input class="form-check-input" type="radio" name="exampleRadios" id="exampleRadios3" value="option3" disabled>
								<label class="form-check-label" for="exampleRadios3">
									Disabled radio
							</label>
						</div>
					</fieldset>
					<fieldset class="my-2">
						<legend>Checkboxes</legend>
							<div class="form-check">
								<input class="form-check-input" type="checkbox" value="" id="defaultCheck1">
								<label class="form-check-label" for="defaultCheck1">
									Default checkbox
								</label>
							</div>
							<div class="form-check">
								<input class="form-check-input" type="checkbox" value="" id="defaultCheck2" disabled>
								<label class="form-check-label" for="defaultCheck2">
									Disabled checkbox
							</label>
						</div>
					</fieldset>
				</form>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h4 class="py-1">Validation</h4>
				<form action="" class="was-validated">
					<div class="form-group">
						<label for="uname">Username:</label>
						<input type="text" class="form-control" id="uname" placeholder="Enter username" name="uname" required>
						<div class="valid-feedback">Valid.</div>
						<div class="invalid-feedback">Please fill out this field.</div>
					</div>
					<div class="form-group">
						<label for="pwd">Password:</label>
						<input type="password" class="form-control" id="pwd" placeholder="Enter password" name="pswd" required>
						<div class="valid-feedback">Valid.</div>
						<div class="invalid-feedback">Please fill out this field.</div>
					</div>
					<div class="form-group form-check">
						<label class="form-check-label">
						<input class="form-check-input" type="checkbox" name="remember" required> I agree on blabla.
						<div class="valid-feedback">Valid.</div>
						<div class="invalid-feedback">Check this checkbox to continue.</div>
						</label>
					</div>
					<button type="submit" class="btn btn-primary">Submit</button>
				</form>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h2 class="py-3">Tables</h2>
				<table class="table">
					<thead>
						<tr>
							<th>#</th>
							<th class="sortable">Name</th>
							<th class="sortable"> <i class="fa fa-envelope"></i> Mail</th>
							<th class="sortable"> <i class="fa fa-phone"></i> Phone</th>
							<th class="sortable text-right">Outstanding</th>
							<th class="text-right">Functions</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>Johnny Avlony</td>
							<td>info@johnnyavlony.com</td>
							<td>(740) 841-7566</td>
							<td class="text-right">$2,400.00</td>
							<td class="text-right">
								<button type="button" class="btn btn-success"><i class="fas fa-edit"></i></button>
            					<button type="button" class="btn btn-danger"><i class="far fa-trash-alt"></i></button>
							</td>
						</tr>
						<tr>
							<td>2</td>
							<td>Johnny Avlony</td>
							<td>info@johnnyavlony.com</td>
							<td>(740) 841-7566</td>
							<td class="text-right">$2,400.00</td>
							<td class="text-right">
								<button type="button" class="btn btn-success"><i class="fas fa-edit"></i></button>
            					<button type="button" class="btn btn-danger"><i class="far fa-trash-alt"></i></button>
							</td>
						</tr>
						<tr class="selected">
							<td>3</td>
							<td>Johnny Avlony</td>
							<td>info@johnnyavlony.com</td>
							<td>(740) 841-7566</td>
							<td class="text-right">$2,400.00</td>
							<td class="text-right">
								<button type="button" class="btn btn-success"><i class="fas fa-edit"></i></button>
            					<button type="button" class="btn btn-danger"><i class="far fa-trash-alt"></i></button>
							</td>
						</tr>
						<tr class="inactive">
							<td>4</td>
							<td>Johnny Avlony</td>
							<td>info@johnnyavlony.com</td>
							<td>(740) 841-7566</td>
							<td class="text-right">$2,400.00</td>
							<td class="text-right">
								<button type="button" class="btn btn-success"><i class="fas fa-edit"></i></button>
            					<button type="button" class="btn btn-danger"><i class="far fa-trash-alt"></i></button>
							</td>
						</tr>
					</tbody>
					<tfoot>
						<tr>
							<td></td>
							<td> </td>
							<td> </td>
							<td> </td>
							<td class="text-right">$15,500.00</td>
							<td class="text-right"> </td>
						</tr>
					</tfoot>
				</table>
			</div>
		</div>

		<div class="row py-2">
			<div class="col">
				<h2 class="py-1">Tags / Badges</h2>
				<span class="badge badge-pill badge-primary">Primary</span>
				<span class="badge badge-pill badge-secondary">Secondary</span>
				<span class="badge badge-pill badge-success">Success</span>
				<span class="badge badge-pill badge-danger">Danger</span>
				<span class="badge badge-pill badge-warning">Warning</span>
				<span class="badge badge-pill badge-info">Info</span>
				<span class="badge badge-pill badge-light">Light</span>
				<span class="badge badge-pill badge-dark">Dark</span>

				<div class="my-2">
					<a href="#" class="badge badge-primary">Primary</a>
					<a href="#" class="badge badge-secondary">Secondary</a>
					<a href="#" class="badge badge-success">Success</a>
					<a href="#" class="badge badge-danger">Danger</a>
					<a href="#" class="badge badge-warning">Warning</a>
					<a href="#" class="badge badge-info">Info</a>
					<a href="#" class="badge badge-light">Light</a>
					<a href="#" class="badge badge-dark">Dark</a>
				</div>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h2 class="py-1">Progress bars</h2>
				<fieldset>
					<legend>Normal</legend>
					<div class="my-2 progress">
						<div class="progress-bar bg-success" role="progressbar" style="width: 25%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar bg-info" role="progressbar" style="width: 50%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar bg-warning" role="progressbar" style="width: 75%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar bg-danger" role="progressbar" style="width: 100%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
				</fieldset>
				<fieldset>
					<legend>Stripped</legend>
					<div class="my-2 progress">
						<div class="progress-bar progress-bar-striped" role="progressbar" style="width: 10%" aria-valuenow="10" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar progress-bar-striped bg-success" role="progressbar" style="width: 25%" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar progress-bar-striped bg-info" role="progressbar" style="width: 50%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar progress-bar-striped bg-warning" role="progressbar" style="width: 75%" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
					<div class="my-2 progress">
						<div class="progress-bar progress-bar-striped bg-danger" role="progressbar" style="width: 100%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
					</div>
				</fieldset>
				<fieldset>
					<legend>Animated</legend>
					<div class="my-2 progress">
  						<div class="progress-bar progress-bar-striped progress-bar-animated" role="progressbar" aria-valuenow="75" aria-valuemin="0" aria-valuemax="100" style="width: 75%"></div>
					</div>
				</fieldset>
			</div>
		</div>
		<div class="row py-2">
			<div class="col">
				<h2 class="py-1">Cards</h2>
				<fieldset>
					<div class="row py-2">
						<div class="col">
							<div class="card">
								<div class="card-header">
									Featured
								</div>
								<div class="card-body">
									<h5 class="card-title">Special title treatment</h5>
									<p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
									<a href="#" class="btn btn-primary">Go somewhere</a>
								</div>
							</div>
						</div>
					</div>
					<div class="row py-2">
						<div class="col-sm-4">
							<div class="card">
							<div class="card-body">
								<h5 class="card-title">Special title treatment</h5>
								<p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
								<a href="#" class="btn btn-primary">Go somewhere</a>
							</div>
							</div>
						</div>
						<div class="col-sm-4">
							<div class="card">
							<div class="card-body">
								<h5 class="card-title">Special title treatment</h5>
								<p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
								<a href="#" class="btn btn-primary">Go somewhere</a>
							</div>
							</div>
						</div>
						<div class="col-sm-4">
							<div class="card" style="width: 18rem;">
								<div class="card-header">
									Featured
								</div>
								<ul class="list-group list-group-flush">
									<li class="list-group-item">Cras justo odio</li>
									<li class="list-group-item">Dapibus ac facilisis in</li>
									<li class="list-group-item">Vestibulum at eros</li>
								</ul>
							</div>
						</div>
					</div>
					<div class="row py-2">
						<div class="col-sm-4">
							<div class="card" style="width: 18rem;">
								<img class="card-img-top" src="https://images.unsplash.com/photo-1562101806-b8ebd0e33011?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=1350&q=80" alt="Card image cap">
								<div class="card-body">
									<h5 class="card-title">Card title</h5>
									<p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
									<a href="#" class="btn btn-primary">Go somewhere</a>
								</div>
							</div>
						</div>
						<div class="col-sm-4">
							<div class="card border-primary mb-3" style="max-width: 18rem;">
								<div class="card-header">Header</div>
								<div class="card-body text-primary">
									<h5 class="card-title">Primary card title</h5>
									<p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
								</div>
							</div>
						</div>
						<div class="col-sm-4">
							<div class="card" style="width: 18rem;">
								<div class="card-body">
									<h5 class="card-title">Special title treatment</h5>
									<p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
									<a href="#" class="btn btn-primary">Go somewhere</a>
								</div>
							</div>
						</div>
					</div>
				</fieldset>
			</div>
		</div>
	</div>												
</template>

<script>
	export default {
		methods: {
		}
	};
</script>

<style lang="scss" scoped>
</style>