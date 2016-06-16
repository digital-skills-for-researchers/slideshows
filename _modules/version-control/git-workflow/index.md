---
layout: slideshow
title: Repositories
slides:

  - content: |

      # Git Workflow
      _Introducing Git into your daily routine_

    notes: |

      :)



  - content: |

      Edit -> Stage -> Commit


  - content: |

      - **Edit** 
      - Stage
      - Commit
      {:.horizontal-list}

      Make changes to your files and save them.
      Create new files or delete existing ones.

    notes: |

      We are all familiar with the "edit" part of the workflow. This is where you make changes to your files and save them just like normal.

  - content: |

      - Edit
      - **Stage**
      - Commit
      {:.horizontal-list}

      Choose the files which should be grouped as 
      an easily-described change or unit of progress.

    notes: |

      At the "stage" part of the workflow, we select the files we're happy with and want to add to our repository for backup. Usually, this consists of all changes since the last commit.

      When staging files, the project should be in a working state without obvious errors.



  - content: |

      - Edit 
      - Stage
      - **Commit**
      {:.horizontal-list}

      Save the staged changes to your repository.

    notes: |

      The "commit" part of the workflow takes all of your staged changes and saves them to the repository.

      By only staging and committing files which are in a functioning state, your repository should always contain a version of your project which at least *works*, even if you don't think it works particularly *well*.



  - content: |

      ## Each commit is a local backup
      A commit is labeled with its author (you!)
      along with the date and time it was created.


  - content: |

      ## A good commit...

      - Achieves only a small piece of progress
      - Changes the code as little as possible
      - Describes the change with a concise message
      - Leaves the project better than it was




---


## The Git Workflow


## A Commit is a local backup



## A Push is a remote backup
It pushes all of your commits to GitHub