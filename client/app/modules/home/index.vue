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
				<fieldset>
					<legend>Small</legend>
					<div class="content buttons">
						<div class="progressbar small">
							<div class="progress" style="width: 15%;"></div>
						</div><br/>
						<div class="progressbar small success stripped">
							<div class="progress" style="width: 40%;">40% complete...</div>
						</div><br/>
						<div class="progressbar small warning stripped animate">
							<div class="progress" style="width: 60%;">60%</div>
						</div>
					</div>
				</fieldset>
				<fieldset>
					<legend>Large</legend>
					<div class="content buttons">
						<div class="progressbar large">
							<div class="progress" style="width: 15%;"></div>
						</div><br/>
						<div class="progressbar large success stripped">
							<div class="progress" style="width: 40%;">40% complete...</div>
						</div><br/>
						<div class="progressbar large warning stripped animate">
							<div class="progress" style="width: 60%;">60%</div>
						</div>
					</div>
				</fieldset>
			</div>
		</div>

		<div class="row py-2">
			<div class="col">
				<h2 class="py-1">Panels & Cards</h2>
				
			</div>
		</div>
		
		<section>
			<h2><span class="number">9.</span><span class="text">Panels & Cards</span></h2>
			<fieldset>
				<legend>Normal Panels</legend>
				<div class="content flex align-center justify-space-around panels">
					<div class="panel">
						<div class="header">Panel normal</div>
						<div class="body">
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
					</div>
					<div class="panel primary">
						<div class="ribbon right red"> <span>Primary</span></div>
						<div class="header">Panel primary</div>
						<div class="body">
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
					</div>
					<div class="panel success" style="height: 332px;">
						<div class="header">Panel success with list</div>
						<div class="body">
							<div class="list">
								<div class="item"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" />
									<div class="body"><strong>Message title <small class="text-muted">John Doe</small></strong>
										<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis eligendi mollitia ratione fugiat earum qui sit vero nisi pariatur eaque quasi reprehenderit possimus consequatur commodi cum quod, amet sed cupiditate?</p>
									</div>
									<div class="footer text-right"><small class="text-muted">1 min ago</small></div>
								</div>
								<div class="item"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" />
									<div class="body"><strong>Message title <small class="text-muted">John Doe</small></strong>
										<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis eligendi mollitia ratione fugiat earum qui sit vero nisi pariatur eaque quasi reprehenderit possimus consequatur commodi cum quod, amet sed cupiditate?
											Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eum perferendis sapiente non atque qui quis pariatur impedit ea cupiditate culpa repellat voluptate, ipsam id illo incidunt nam commodi optio? Quasi.</p>
									</div>
									<div class="footer text-right"><small class="text-muted">3 min ago</small></div>
								</div>
								<div class="item"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" />
									<div class="body"><strong>Message title <small class="text-muted">John Doe</small></strong>
										<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis eligendi mollitia ratione fugiat earum qui sit vero nisi.</p>
									</div>
									<div class="footer text-right"><small class="text-muted">15 min ago</small></div>
								</div>
								<div class="item"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" />
									<div class="body"><strong>Message title <small class="text-muted">John Doe</small></strong>
										<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis eligendi mollitia ratione fugiat earum qui sit vero nisi pariatur eaque quasi reprehenderit possimus consequatur commodi cum quod, amet sed cupiditate?</p>
									</div>
									<div class="footer text-right"><small class="text-muted">3 hours ago</small></div>
								</div>
								<div class="item"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" />
									<div class="body"><strong>Message title <small class="text-muted">John Doe</small></strong>
										<p class="text-justify">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Facilis eligendi mollitia ratione fugiat earum qui sit vero nisi pariatur eaque quasi reprehenderit possimus consequatur commodi cum quod, amet sed cupiditate?
											Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nemo officia, nulla ad quae. Possimus, necessitatibus excepturi ad vel aspernatur ipsam molestiae. Blanditiis assumenda, doloribus tenetur inventore,
											earum fugiat! Ducimus, recusandae.</p>
									</div>
									<div class="footer text-right"><small class="text-muted">1 day ago</small></div>
								</div>
							</div>
						</div>
					</div>
				</div>
				<div class="content flex align-center justify-space-around panels">
					<div class="panel warning" style="max-height: 280px; max-width: 600px;">
						<div class="header">Panel warning with scroll</div>
						<div class="body">
							<p>Duis ex nulla eu ex quis consectetur amet voluptate qui ipsum aliqua nisi commodo cupidatat. Reprehenderit aliqua sint magna ad eiusmod magna non esse. Ex tempor ex duis dolore commodo labore aliquip ad dolor nulla est. Ex
								eiusmod labore deserunt velit ad consequat elit. Quis elit cupidatat culpa pariatur excepteur. Elit nulla nisi ut nulla cupidatat ipsum officia sint consectetur in laboris.</p>
							<p>Voluptate anim in et esse. Voluptate ad est irure eiusmod sit enim pariatur adipisicing. Dolore officia nulla reprehenderit ipsum do aliquip incididunt eiusmod cupidatat exercitation consectetur incididunt.</p>
						</div>
						<div class="footer">Panel footer</div>
					</div>
					<div class="panel danger">
						<div class="header">Panel danger</div>
						<div class="body">
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque.</p>
						</div>
						<div class="footer">Panel footer</div>
					</div>
					<div class="panel outline">
						<div class="header">Panel outline</div>
						<div class="body">
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
					</div>
				</div>
			</fieldset>
			<fieldset>
				<legend>Normal cards</legend>
				<div class="content flex align-center justify-space-around panels">
					<div class="card">
						<div class="block">
							<div class="title">Simple Card</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
						<div class="block"><small class="text-muted">Last updated 5 mins ago</small></div>
					</div>
					<div class="card">
						<div class="ribbon right orange"> <span>-20%</span></div><img class="img" src="http://lorempixel.com/350/150/city" />
						<div class="block">
							<div class="title">Card with image</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
						<div class="block"><button class="button success">Checkout</button></div>
					</div>
					<div class="card">
						<div class="ribbon left primary"> <span>Brand new</span></div><img class="img" src="http://placehold.it/350x150" />
						<div class="block">
							<div class="title">Card Title wih ribbon</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.</p>
						</div>
						<div class="block text-right"><button class="button danger">DELETE</button><button class="button outline">Close</button></div>
					</div>
				</div>
			</fieldset>
			<fieldset>
				<legend>Cards in columns</legend>
				<div class="content card-columns">
					<div class="card">
						<div class="block">
							<div class="title">Small Card 1</div>
							<p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quos repellendus architecto molestiae iure enim labore dolores similique, quia consequatur culpa, at cumque ad tenetur nemo vitae dolorem ipsum repellat optio! <a class="link"
									href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 2</div>
							<p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Porro voluptate, neque voluptatibus mollitia aliquid, harum in laborum non amet cupiditate ea nisi necessitatibus quis! Earum architecto corporis molestiae nihil molestias?
								Lorem ipsum dolor sit amet, consectetur adipisicing elit. Ut, voluptate. Eaque nisi alias consectetur ipsum eveniet qui esse repellat voluptas mollitia, obcaecati corporis a modi officia, architecto commodi eius sint!
								<a
									class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a>
							</p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 3</div>
							<p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. <a class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card"><img class="img" src="http://lorempixel.com/600/300/city" />
						<div class="block">
							<div class="title">Small Card 4</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa</p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 5</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa <a class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
						<div class="block"><button class="button success">Checkout</button></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 6</div>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa </p>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt voluptatum quos autem magnam doloribus sunt. Atque quas accusamus repellat, odio dolore sapiente voluptatibus nemo numquam eum odit tempore, similique natus!
								<a class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 7</div>
							<p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa <a class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
					<div class="card">
						<div class="block">
							<div class="title">Small Card 8</div>
							<p> Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa <a class="link" href="https://twitter.com/Icebobcsi">@Icebobcsi</a></p>
						</div>
						<div class="block"><small class="text-muted">08:45 PM - 14 Jun 2016</small></div>
					</div>
				</div>
			</fieldset>
		</section>
		<section>
			<h2><span class="number">10.</span><span class="text">Media</span></h2>
			<fieldset>
				<legend>Normal media</legend>
				<div class="content list">
					<div class="media">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								</p>
							<p>Elit ex id excepteur aliqua sint et culpa nisi laborum. Cupidatat anim aliqua nisi tempor nisi sint mollit non elit laboris consequat. Ut sint mollit voluptate quis sunt magna voluptate incididunt amet voluptate aute occaecat
								nulla. Nostrud ut eiusmod duis consequat sunt proident in aute esse adipisicing cupidatat commodo consequat dolor. Irure minim consectetur est duis nulla aliqua fugiat culpa proident cupidatat elit magna. Dolor esse magna
								pariatur sint adipisicing cupidatat veniam excepteur aliquip. Qui fugiat non eiusmod do sunt excepteur enim aliquip reprehenderit ullamco.<a class="link" href="#"> Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
					<div class="media primary">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								<a class="link" href="#">Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
					<div class="media success">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								<a class="link" href="#">Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
					<div class="media warning">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								<a class="link" href="#">Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
					<div class="media danger">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								<a class="link" href="#">Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
					<div class="media outline">
						<div class="media-left"><img class="avatar" src="https://s3.amazonaws.com/uifaces/faces/twitter/kolage/73.jpg" /></div>
						<div class="media-content"><strong>John Doe</strong><small class="text-muted">@johndoe - 31m ago</small>
							<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Consequuntur dicta cumque assumenda culpa maiores omnis totam obcaecati voluptas eligendi sapiente enim debitis, illo dolore facilis, in, nihil perspiciatis, et perferendis.
								<a class="link" href="#">Read more...</a></p>
							<div class="functions"><a href="#"><i class="fa fa-reply"></i></a><a href="#"><i class="fa fa-heart"></i></a><a href="#"><i class="fa fa-trash"></i></a></div>
						</div>
						<div class="media-right"><a class="close" href="#" title="Close"></a></div>
					</div>
				</div>
			</fieldset>
		</section>
	</div>												
</template>

<script>
	export default {

		methods: {
			getTypographyInfo(elType) {
				if (this.$el) {
					let element = this.$el.querySelector(elType);
					if (element) {
						let style = window.getComputedStyle(element, null);
						return style.fontFamily.split(",")[0] + " " + style.fontWeight + ", " + style.fontSize;
					}
				}
			}
		}
	};

</script>

<style lang="scss" scoped>
	// @import "../../../scss/themes/blurred/variables";

	// .container {
	// 	padding: 0 1rem;
	// }

	// section {
	// 	&:not(:last-child) {
	// 		margin-bottom: 40px;
	// 	}

	// 	> h2 {
	// 		font-size: 1.5rem;
	// 		margin-bottom: 20px;
	// 		padding: 8px 10px;
			
	// 		background-color: rgba(darken($backgroundColor, 10%), 0.6);
	// 		border: 1px solid darken($backgroundColor, 8%);
	// 		border-radius: 8px;
			
	// 		.number {
	// 			color: #888;
	// 		}
			
	// 		.text {
	// 			margin-left: 4px;
	// 			font-weight: $fontLight;
	// 			text-transform: uppercase;
	// 		}
			
	// 		clear: both;
			
	// 	} // .title

	// } //. section	

	// .buttons {
	// 	margin-bottom: 20px;
	// }

	// .list {
	// 	> * {
	// 		margin-bottom: 20px;
	// 	}
	// }

	// .panels {
	// 	align-items: flex-start;
	// 	.panel, .card {
	// 		margin: 20px;
	// 	}

	// 	.card {
	// 		max-width: 350px;
	// 	}
	// }

	// .colors {
	// 	$boxSize: 150px;

	// 	.box {
	// 		width: $boxSize;
	// 		height: $boxSize + 20px;

	// 		border: 1px solid darken($backgroundColor, 10%);
	// 		border-radius: 6px;

	// 		margin: 5px 20px;
	// 		padding: 2px;
			
	// 		.caption {
	// 			float: left;
	// 			width: 100%;
	// 			text-align: center;
	// 		}

	// 		.main {
	// 			float: left;
	// 			width: 100%;
	// 			height: $boxSize - 60px;
	// 		} // .main
			
	// 		.light {
	// 			float: left;
	// 			width: 50%;
	// 			height: 30px;
				
	// 		} // .light

	// 		.dark {
	// 			float: right;
	// 			width: 50%;
	// 			height: 30px;
				
	// 		} // .dark
			
	// 		.code {
	// 			float: left;
	// 			width: 100%;
	// 			position: relative;
	// 			margin-top: 5px;
				
	// 			&:after {
	// 				position: absolute;
	// 				top: 0; bottom: 0;
	// 				left: 0; right: 0;
	// 				margin: auto;
	// 				width: 100%;
	// 				text-align: center;
	// 				font-family: "Consolas";
	// 				color: White;
	// 			}
	// 		} // .code

	// 		$colors: $color1, $color2, $color3, $color4, $color5;

	// 		$colors-light: $color1-light, $color2-light, $color3-light, $color4-light, $color5-light;
	// 		$colors-dark: $color1-dark, $color2-dark, $color3-dark, $color4-dark, $color5-dark;

	// 		@for $i from 1 through 5 {

	// 			$c: nth($colors, $i);

	// 			&.box#{$i} { 
	// 				.main { background-color: $c; } 
	// 				.light { background-color: nth($colors-light, $i); }
	// 				.dark { background-color: nth($colors-dark, $i); }
	// 				.code:after {	content: "" + $c; }

	// 			} // box
				
	// 		} // for
			
	// 	} // .box
		
	// } // .colors
</style>