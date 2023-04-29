<template>
    <div class="home">

        <form class="main_form">
            <h5>Add Movie Details</h5>
            <p>Ensure all details are filled correctly</p>

            <div class="formgroup mt-5">
                <div class="row">
                    <div class="col-6 ">
                        <input type="text" placeholder="Movie Title" class="form-control">
                    </div>
                    <div class="col-6 ">
                        <select class="form-control">
                            <option>Afro</option>
                            <option>English</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Language</label>
                        <select class="form-control">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        
                        <label>Genre</label>
                        <select class="form-control">
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Wood</label>
                        <select class="form-control">
                            <option>Nollywood</option>
                            <option>Bollywood</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Type</label>
                        <select class="form-control">
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Ratings</label>
                        <select class="form-control">
                            <option>1</option>
                            <option>2</option>
                            <option>3</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Original Language</label>
                        <select class="form-control">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Language</label>
                        <select class="form-control">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Genre</label>
                        <select class="form-control">
                            <option>Genre</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Movie Original Language</label>
                        <select class="form-control">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Symposis</label>
                        <input type="text" placeholder="Symposis" class="form-control">

                    </div>

                </div>
            </div>

            <div class="formcontrol mt-4">
                <label style="font-weight: 500;">Movie Type</label>
                <div class="row mt-3">
                    <div class="col-sm-4">
                        <input type="radio" id="option1" name="options" value="option1">
                        <label for="option1" style="margin-left: 20px;"> Single Movie </label><br>
                    </div>
                    <div class="col-sm-4">
                        <input type="radio" id="option2" name="options" value="option2">
                        <label for="option2" style="margin-left: 20px;"> Multi Part</label>
                    </div>
                    <div class="col-sm-4">
                        <input type="radio" id="option3" name="options" value="option3">
                        <label for="option3" style="margin-left: 20px;">Series</label><br>
                    </div>
                </div>
            </div>

            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-4">
                        <input type="text" placeholder="Year Produces" class="form-control">

                    </div>
                    <div class="col-4">
                        <select class="form-control">
                            <option>Executive Producer</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <select class="form-control">
                            <option>Production Company</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>


            <div class="formgroup mt-4">
                <ul class="nav nav-tabs nav-fill mb-3 mt-3" id="ex1" role="tablist">
                    <li class="nav-item" role="presentation">
                        <a class="nav-link active" id="ex2-tab-1" data-bs-toggle="tab" href="#ex2-tabs-1" role="tab"
                            aria-controls="ex2-tabs-1" aria-selected="true">Single Movie</a>
                    </li>
                    <li class="nav-item" role="presentation">
                        <a class="nav-link" id="ex2-tab-2" data-bs-toggle="tab" href="#ex2-tabs-2" role="tab"
                            aria-controls="ex2-tabs-2" aria-selected="false">Multi Movie</a>
                    </li>
                    <li class="nav-item" role="presentation">
                        <a class="nav-link" id="ex2-tab-3" data-bs-toggle="tab" href="#ex2-tabs-3" role="tab"
                            aria-controls="ex2-tabs-3" aria-selected="false">Series Movie</a>
                    </li>
                </ul>
                <div class="tab-content" id="ex2-content">
                    <div class="tab-pane fade show active" id="ex2-tabs-1" role="tabpanel" aria-labelledby="ex2-tab-1">
                        <input type="text" placeholder="Duration" class="form-control">
                    </div>
                    <div class="tab-pane fade" id="ex2-tabs-2" role="tabpanel" aria-labelledby="ex2-tab-2">
                        <div class="row">
                            <div class="col-6">
                                <input type="text" placeholder="Number Of Parts" class="form-control">
                            </div>
                            <div class="col-6">
                                <input type="text" placeholder="Duration" class="form-control">
                            </div>
                        </div>
                    </div>
                    <div class="tab-pane fade" id="ex2-tabs-3" role="tabpanel" aria-labelledby="ex2-tab-3">
                        <div class="row">
                            <div class="col-4">
                                <input type="text" placeholder="Number Of Seasons" class="form-control">
                            </div>
                            <div class="col-4">
                                <input type="text" placeholder="Season 1 Episodes" class="form-control">
                            </div>
                            <div class="col-4">
                                <input type="text" placeholder="Duration (total) S1E1:" class="form-control">
                            </div>
                        </div>
                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <label style="font-weight: 500;">Initial Reviewers</label>
                <div class="row mt-3">
                    <div class="col-sm-4">
                        <label>Pre-acquisition Reviewer</label>
                        <input type="date" placeholder="Date" class="form-control">
                    </div>
                </div>


            </div>

            <div class="formgroup mt-4">
                <label style="font-weight: 500;">Time Reviewed</label>
                <div class="row mt-3">
                    <div class="col-6 ">
                        <label>From</label>
                        <input type="date" placeholder="Year Produces" class="form-control">
                    </div>
                    <div class="col-6 ">
                        <label>To</label>
                        <input type="date" placeholder="Year Produces" class="form-control">
                    </div>
                </div>
            </div>
            <div class="formgroup mt-4">
                <label style="font-weight: 500;">Approval</label>
                <div class="row mt-3">
                    <div class="col-sm-6">
                        <input type="checkbox" id="option1" name="options[]" value="option1" @change="open_approval()">
                        <label for="approve" style="margin-left: 20px;"> Approved </label><br>
                    </div>
                    <div class="col-sm-6">
                        <input type="checkbox" id="option2" name="options[]" value="option2">
                        <label for="approve2" style="margin-left: 20px;">Not Approved</label>
                    </div>
                </div>
            </div>
            <div class="formgroup mt-4">
                <textarea name="" id="" cols="20" rows="2" class="form-control"
                    placeholder="Reasons For Approval or Non Approval"></textarea>
            </div>

            <div class="approval_det mt-3" v-if="isVisible">
                <div class="formgroup mt-2">
                    <label class="mb-3">Approved By</label>
                    <input type="text" placeholder="Name" class="form-control">
                </div>

                <label style="font-weight: 500; margin-top: 10px">Trailers</label>

                <div class="formgroup mt-2">
                    <label>Language</label>
                    <select class="form-control">
                        <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                    </select>


                </div>

                <div class="formgroup mt-4">
                    <div class="row">
                        <div class="col-6 ">
                            <label>Approved By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-3">

                        </div>
                        <div class="col-6 ">
                            <label>Date Approved</label>
                            <input type="date" placeholder="Approved By" class="form-control mt-3">

                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">

                    <label>Location/Link</label>
                    <input type="text" placeholder="Location/link" class="form-control mt-3">


                </div>

                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Posters</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>


                </div>

                <div class="formgroup mt-4">
                    <label>Assigned To</label>
                    <input type="text" placeholder="Assigned To" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>


                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Language 1:</label>
                            <input type="text" placeholder="Done By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Approved By</label>
                            <input type="text" placeholder="" class="form-control mt-2">
                        </div>
                    </div>

                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Date Approved</label>
                            <input type="date" placeholder="Done By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Location/Link</label>
                            <input type="text" placeholder="" class="form-control mt-2">
                        </div>
                    </div>

                </div>

                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Actors</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Actors Name</label>
                            <input type="text" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>

                </div>


                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Movie Compression & Watermarking</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Date Compressed/Watermarked</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Language Compressed/Watermarked</label>

                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Compressed/watermarked by</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>

                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Movie SRT Transcription</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Assiged To</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Transcriber</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Transcription language</label>
                            <select class="form-control mt-2">
                                <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                            </select>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Approved By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>


                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Trailer SRT Transcription</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Assiged To</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Transcriber</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Transcription language</label>
                            <select class="form-control mt-2">
                                <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                            </select>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Approved By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>




                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Synopsis Translation</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Assiged To</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Transcriber</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Transcription language</label>
                            <select class="form-control mt-2">
                                <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                            </select>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Approved By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>




                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Movie Dubbing</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Assiged To</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Dubber</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Transcription language</label>
                            <select class="form-control mt-2">
                                <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                            </select>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Approved By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Dubbing Credit </label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Name</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Character</label>
                            <input type="text" placeholder="character" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <!--            <div class="formgroup mt-4">

                    <label style="font-weight: 500;">Classifications (Choose all that apply – Indicate if language is
                        embedded)</label>
                    <div class="row mt-3">
                        <div class="col-6 ">
                            <select class="form-control">
                                <option>Afro</option>
                                <option>English</option>
                                <option>French</option>
                            </select>

                        </div>
                        <div class="col-6 ">
                            <select class="form-control">
                                <option>Language</option>
                                <option>English</option>
                                <option>French</option>
                            </select>

                        </div>
                    </div>

                </div>
                <div class="formgroup mt-4">
                    <div class="row">

                        <div class="col-6 ">
                            <select class="form-control">
                                <option>Genre</option>
                                <option>Spanish</option>
                                <option>French</option>
                            </select>

                        </div>
                        <div class="col-6 ">
                            <select class="form-control">
                                <option>Wood</option>
                                <option>Nollywood</option>
                                <option>Bollywood</option>
                            </select>

                        </div>
                    </div>

                </div>
                <div class="formgroup mt-4">
                    <div class="row">

                        <div class="col-12 ">
                            <select class="form-control">
                                <option>Type</option>
                                <option>Spanish</option>
                                <option>French</option>
                            </select>

                        </div>
                    </div>

                </div>
 -->




                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Trailer Dubbing</label>
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Assigned Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Assigned Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>
                <div class="formgroup mt-4">
                    <label> Assiged To</label>
                    <input type="text" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Completed Date</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Completed Time</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Dubber</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Dubbed language</label>
                            <select class="form-control mt-2">
                                <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                            </select>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Authorized By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Authorization Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>


                <div class="formgroup mt-4">
                    <label style="font-weight: 500;">Payment</label> <br>
                    <label class="mt-3">Purchase Amount </label>
                    <input type="date" placeholder="" class="form-control mt-2">
                </div>
                <div class="formgroup mt-4">
                    <div class="row">
                        <div class="col-sm-6">
                            <label>Invoice Date</label>
                            <input type="text" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Invoice Number</label>
                            <input type="text" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>

                </div>
                <div class="formgroup mt-4">

                    <div class="row ">
                        <div class="col-sm-6">
                            <label>Date Paid</label>
                            <input type="date" placeholder="Date" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Amount Paid</label>
                            <input type="text" placeholder="Date" class="form-control mt-2">
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">

                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Entity Paid</label>
                            <input type="text" placeholder="Entity Paid" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Authorization Received</label>
                            <div class="row">
                                <div class="col-sm-6 mt-3">

                                    <input type="radio" id="author1" name="authors" value="author1">
                                    <label for="author1" style="margin-left: 20px;"> Yes </label><br>

                                </div>
                                <div class="col-sm-6 mt-3">

                                    <input type="radio" id="author2" name="authors" value="author2">
                                    <label for="author2" style="margin-left: 20px;"> No </label><br>

                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="formgroup mt-4">
                    <div class="row mt-3">
                        <div class="col-sm-6">
                            <label>Authorized By</label>
                            <input type="text" placeholder="Approved By" class="form-control mt-2">
                        </div>
                        <div class="col-sm-6">
                            <label>Authorization Location/link</label>
                            <input type="text" placeholder="Location/link" class="form-control mt-2">
                        </div>
                    </div>
                </div>





            </div>




            <div class="formgroup mt-4">
                <button class="btn">Submit</button>
            </div>






        </form>



    </div>
</template>

<script  setup>

import { ref } from 'vue';

import { languagesAll, countries } from 'countries-list';

definePageMeta({
    layout: 'nav'
})
const isVisible = ref(false)

const open_approval = () => {
    isVisible.value = !isVisible.value
}

</script>


<style scoped>
.home {
    background: white;
    height: 100vh;
    overflow: auto;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;
    margin: 0px;
    padding: 0px;
    -ms-overflow-style: none !important;
    /* for Internet Explorer, Edge */
    width: 100%;
}

.home_page {
    background: whitesmoke;
    height: 100vh;
    overflow: auto;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;
    margin: 0px;
    padding: 0px;
    -ms-overflow-style: none !important;
    /* for Internet Explorer, Edge */
    width: 100%;
}

.main_form {
    width: 80%;
    margin: auto;
    margin-top: 5rem;
}

.main_form h5,
.main_form p {
    text-align: center;
}

.formgroup input:focus,
.formgroup select:focus,
.formgroup textarea:focus {
    box-shadow: none;
    outline: none;
}

.formgroup button {
    display: block;
    width: 50%;
    margin: auto;
    color: white;
    background: #FB0A03;
    ;
}
</style>